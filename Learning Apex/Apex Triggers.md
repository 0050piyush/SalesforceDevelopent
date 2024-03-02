# Apex Triggers
Benefit of Apex Triggers Over other Automation Tools:

&rarr; Though we have automation tools like Workflow, Process Builder, Flow but all of these have some or other limitations therefore
its very much possible that all complex tasks of real time project can't be achieved with the help of these point & click tools
so in order to achieve the complex requirements of the RTP , we use apex triggers because it has got no limitation and it can
solve pretty much every possible RTP scenarios.

&rarr; Helps in building any kind of automation

&rarr; Can be used in making complex validations by using addError() (i.e. All those complex Validations, which can't be achieved
through Validation rules can easily be achieved through triggers)

&rarr; Are extremely fast (as compared to workflow , Process Builder, Flow)

Ex. Of complex requirement in which triggers can be very useful:

- When Product Sale is completes then

1. Generate its bill and send to the clients

2. Send the shipment details to the Seller etc

## Apex Triggers vs Apex Classes

**Apex Trigger**

A trigger is Apex code that executes before or after
specific data manipulation language (DML) events
occur, such as before object records are inserted
into the database, or after records have been
deleted. A trigger is associated with a standard or
custom object and can call methods of Apex classes.
Triggers are related to a single Object at a time (like
Record-Triggered Flows).
Triggers are constructed with one or more events
(before insert, after delete, etc).

**Apex Class**

An Apex class is a template or blueprint from which
Apex objects are created. Classes consist of other
classes, user-defined methods, variables, exception
types, and static initialization code. In this case, an
‘Apex object’ is just an instance of a Class.
Use Apex Classes to extend triggers, and break your
code down into bite-sized, manageable chunks
(similar to Sub Flows).
To define your class you need to set an access
modifier (private/public/global), give your class a
name, and set any parameters.

## Trigger Context & Context Variables

Why Do we need a context variables ??

Trigger ContactTrigger on Contact (before insert,After Insert,before update, After update,Before
Delete,After Delete,After UnDelete) 
```java
{
    system.debug('Trigger Invoked at the time of Before Insert');
    system.debug('Trigger Invoked at the time of After Insert');
    system.debug('Trigger Invoked at the time of Before Update');
    system.debug('Trigger Invoked at the time of After Update');
    system.debug('Trigger Invoked at the time of Before Delete');
    system.debug('Trigger Invoked at the time of After Delete');
    system.debug('Trigger Invoked at the time of After UnDelete');
}
```
Any potential problem with the above code ???

Yes – A big Problem , all these lines will execute every single time any one of the above mentioned event
takes place

## Solution to this Problem --> context Variables

Now lets modify the above trigger with the context variable

trigger ContactTrigger on Contact (before insert,After Insert,before update, After update,Before Delete,After Delete,After UnDelete) 

```java
{
for(Contact contactRecord : Trigger.new)
{
if (Trigger.isBefore && Trigger.isInsert)
{
system.debug('Trigger Invoked at the time Before Insert');
}
if (Trigger.isAfter && Trigger.isInsert )
{
system.debug('Trigger Invoked at the time After Insert');
}
if (Trigger.isBefore && Trigger.isUpdate)
{
system.debug('Trigger Invoked at the time Before Update');
}
if (Trigger.isAfter && Trigger.isUpdate )
{
system.debug('Trigger Invoked at the time After Update');
}
if (Trigger.isBefore && Trigger.isDelete)
{
system.debug('Trigger Invoked at the time Before Delete');
}
if (Trigger.isAfter && Trigger.isDelete )
{
system.debug('Trigger Invoked at the time After Delete');
}
if (Trigger.isAfter && Trigger.isunDelete )
{
system.debug('Trigger Invoked at the time After unDelete');
}
}
}
```

- **Trigger.New** A List of all records inserted, updated, or undeleted.

- **Trigger.Old** A List of the old versions of the records before they were updated or
deleted.

- **Trigger.NewMap** A Map of all records inserted, updated, or undeleted.

- **Trigger.OldMap** A Map of the old versions of the records before they were updated
or deleted.

- **Trigger.Size** The total number of records in a trigger..

## Three Most Important Things While Writing Triggers

- Always Bulkify: Design your triggers to handle multiple records at once, and remember to use one trigger per object where possible.
(Triggers can handle up to 200 records).

- Limit your usage of SOQL by running before a Loop, then performing logic to the records within a Loop.
(Up to 100 SOQL queries per Transaction).

- Assign variables within a Loop, then run DML afterwards.
(Up to 150 DML executions per Transaction).






















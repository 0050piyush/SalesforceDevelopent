# sObjects

In Apex programming (the programming language used in the Salesforce platform), an SObject, short for "Salesforce Object," represents a record in the Salesforce database. SObjects are similar to objects in other programming languages but are specifically tailored to interact with Salesforce data.

***Here are some key points about SObjects in Apex programming:***

**Representing Database Records:** SObjects are used to represent data records stored in Salesforce databases. These records can be of standard objects provided by Salesforce (such as Account, Contact, Opportunity) or custom objects created by developers.

**Typed Objects:** SObjects are strongly typed objects in Apex. Each SObject corresponds to a specific type (e.g., Account, Contact, CustomObject__c), and developers can define variables of these types to work with records of that type.

**Fields and Relationships:** SObjects have fields that store data, and relationships define how they are related to other SObjects. Fields can be standard fields provided by Salesforce or custom fields defined by developers.

**CRUD Operations:** SObjects support Create, Read, Update, and Delete (CRUD) operations, allowing developers to manipulate records in the Salesforce database using DML (Data Manipulation Language) statements.

**Querying Data:** Developers can use SOQL (Salesforce Object Query Language) to query SObjects and retrieve records from the Salesforce database. SOQL is similar to SQL (Structured Query Language) but tailored for querying Salesforce data.

**Object-Oriented:** SObjects are part of the object-oriented programming paradigm in Apex. Developers can create and manipulate SObjects using object-oriented techniques such as inheritance, polymorphism, and encapsulation.

**Metadata:** SObjects also contain metadata that describes the structure and properties of the objects, including fields, relationships, and other metadata attributes.

In summary, SObjects in Apex programming are the primary means of interacting with Salesforce database records, providing a structured and object-oriented approach to working with Salesforce data within Apex code.

&rarr; Example:
```java
  List <Sobject> objects = new List <Sobject>();
  Account acc1 = new Account(Name = 'My Studies');
  Opportunity opp2 = new Opportunity(name = 'Studies');
  Case case3 = new Case(Status = 'new', Origin = 'Phone');
  // add these records to the list
  // list of sobjects
  objects.add(acc1);
  objects.add(opp2);
  objects.add(case3);
  System.debug('elements in the list are: '+objects);
```

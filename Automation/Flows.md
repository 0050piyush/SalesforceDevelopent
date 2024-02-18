# Flows

In Apex, flows refer to the process of controlling the sequence of execution in a program. This can involve the flow of data, control statements, and interactions between different components of an application. Here's a breakdown of different Types and aspects related to flows in Apex:

## Types 
*There are 5 types of Salesforce flows.*

1. Screen Flow

With Screen Flow you can create a custom UI (user interface) and guide users through a business process that can be launched from Lightning Pages, Experience Cloud (previously known as Community Cloud), quick actions and more.

2. Record-Triggered Flow

Record-Triggered Flow launches when is record is created, updated, or deleted. So far, we have used Apex triggers for these automations some of which can now be done using Flows.

3. Scheduled-Triggered Flow

This flow launches at the specified time and frequency for each record in a batch. Traditionally we have met this kind of requirement using Apex batch jobs.

4. Platform Event Flow

Platform event flow Launches when a platform event message is received. For example, you can pump the data from external system in Platform Events and then use Flows to split and save the records in different objects. 

5. Auto launched Flow

Auto Launches flow launch when invoked by Apex, Process Builder or even REST API.

![Types-of-Flow](https://www.apexhours.com/wp-content/uploads/2021/09/Types-of-Flow.png)

## Aspects

1. Control Flow Statements:

      Apex supports various control flow statements that dictate the sequence in which code is executed. These include:

    - *Conditional Statements:* such as if-else statements, which allow you to execute different blocks of code based on certain conditions.

    - *Looping Statements:* such as for loops, while loops, and do-while loops, which allow you to execute a block of code repeatedly based on certain conditions.

2. Exception Handling:

 Flow control also involves handling exceptions or errors that may occur during the execution of code. Apex provides try-catch-finally blocks for handling exceptions gracefully.

3. Method Invocation:

 Flow control includes invoking methods or functions in a specific order to achieve desired functionality. Methods can be invoked synchronously or asynchronously, depending on the requirements.

4. Data Flow:

 This refers to the flow of data within a program. In Apex, data can flow between variables, objects, and methods. You can manipulate data using various operations such as assignment, arithmetic operations, and method calls.

5. Transaction Control:

 Apex allows you to control transactions, which involve the execution of a series of operations that need to be treated as a single unit of work. You can start, commit, or rollback transactions based on certain conditions.

6. Asynchronous Processing:

 In certain scenarios, you may need to execute code asynchronously, outside the normal flow of execution. Apex provides mechanisms such as future methods, queueable jobs, and batch jobs for asynchronous processing.

7. Governor Limits:

 Apex enforces various governor limits to ensure efficient resource utilization and prevent abuse. These limits control the flow of execution by imposing restrictions on factors such as CPU time, heap size, and DML statements.

8. Integration and External Services:

 Flow control may also involve integrating with external systems or services. This includes making callouts to external APIs, processing responses asynchronously, and handling errors or timeouts.

9. Custom Flows:

 Developers can design custom flows in Apex to orchestrate complex sequences of actions or operations within an application. This involves designing flowcharts or diagrams to represent the desired flow of execution and implementing the corresponding logic in Apex code.

_Overall, flows in Apex encompass various aspects of program control, including control flow statements, exception handling, data flow, transaction control, event-driven programming, asynchronous processing, governor limits, integration with external services, and custom flow design. Understanding and effectively managing these flows is essential for developing robust and efficient Apex applications._

## Salesforce Flow Components

- Interaction
- Logic
- Data Elements

![Salesforce Flow Components](https://www.apexhours.com/wp-content/uploads/2021/09/Flow-Component-in-Salesforce.png)

## Salesforce Flow Limits and Considerations
1. ***Limits per flow interview:*** Executed elements at runtime per flow: 2,000
2. ***General Flow Limits:***
    - Versions per flow: 50
    - Active flows per flow type: 5 in PROFESSIONAL EDITIONS and 2000 in all others
    - Total flows per flow type: 5 in PROFESSIONAL EDITIONS and 4000 in all others
3. ***Per-Transaction Flow Limits:***
    
    - Total number of SOQL queries issued: 100
    - Total number of records retrieved by SOQL queries: 50,000
    - Total number of DML statements issued: 150
    - Total number of records processed as a result of DML statements: 10,000
4. [***Flow Usage-Based Entitlements.***](https://help.salesforce.com/s/articleView?id=sf.flow_considerations_usage_entitlements.htm&type=5)

## What are the best practices of Salesforce Flow Builder?

1. Always! Plan Before You Build
2. No DML Statement In Loops
3. Use The Advanced Technique To Merge Decision Node
4. Build Reusable Flow(S) – Subflow(S)
5. Don’t Create Flow For Everything
6. Build In A Test/Sandbox Environment
7. Supercharge Flow With Invocable Apex
8. Don’t Hardcode IDs, Query For Them!

## What are different flow terms?

1. Lightning Flow: Includes tools for building, managing and running flow and processes.
2. Flow Builder: Point and click tool for builder flows
3. Flow: Application that automates business processes by collecting data and doing something in Salesforce or external System.
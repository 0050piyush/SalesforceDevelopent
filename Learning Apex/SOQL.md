# SOQL
Brief overview of SOQL (Salesforce Object Query Language):

SOQL stands for Salesforce Object Query Language. It is a query language used to search your organization's Salesforce data for specific information. SOQL is similar to SQL (Structured Query Language) but is specifically designed for querying Salesforce's metadata and data models.

With SOQL, you can retrieve records from a single object or from multiple objects that are related to each other through relationships. You can also filter and sort the retrieved data, aggregate results, and perform various operations similar to what you can do with SQL.

SOQL is commonly used in Salesforce development for tasks such as:

1. Retrieving data for reports and dashboards.
2. Displaying data on Salesforce pages and custom applications.
3. Performing data operations within triggers, Apex code, and Visualforce pages.

Overall, SOQL is a powerful tool for querying and manipulating data within the Salesforce platform.

1. **Basic Syntax:**
   ```sql
   SELECT field1, field2 FROM ObjectName WHERE condition
   ```

2. **Selecting All Fields:**
   ```sql
   SELECT * FROM ObjectName
   ```

3. **Filtering Records:**
   - Equals:
     ```sql
     SELECT field1 FROM ObjectName WHERE field2 = 'value'
     ```
   - Not Equals:
     ```sql
     SELECT field1 FROM ObjectName WHERE field2 != 'value'
     ```
   - Greater Than:
     ```sql
     SELECT field1 FROM ObjectName WHERE field2 > 'value'
     ```
   - Less Than:
     ```sql
     SELECT field1 FROM ObjectName WHERE field2 < 'value'
     ```
   - IN Operator:
     ```sql
     SELECT field1 FROM ObjectName WHERE field2 IN ('value1', 'value2')
     ```

4. **Logical Operators:**
   - AND:
     ```sql
     SELECT field1 FROM ObjectName WHERE field2 = 'value' AND field3 = 'value'
     ```
   - OR:
     ```sql
     SELECT field1 FROM ObjectName WHERE field2 = 'value' OR field3 = 'value'
     ```

5. **Sorting Results:**
   ```sql
   SELECT field1 FROM ObjectName ORDER BY field1 ASC/DESC
   ```

6. **Limiting Records:**
   ```sql
   SELECT field1 FROM ObjectName LIMIT number
   ```

7. **Aggregate Functions:**
   - COUNT:
     ```sql
     SELECT COUNT(Id) FROM ObjectName
     ```
   - SUM, AVG, MAX, MIN

8. **Relationship Queries:**
   ```sql
   SELECT Name, (SELECT LastName FROM Contacts) FROM Account
   ```

9. **Date Functions:**
   ```sql
   SELECT field1 FROM ObjectName WHERE CALENDAR_MONTH(field2) = 12
   ```

10. **Group By Clause:**
    ```sql
    SELECT field1, COUNT(Id) FROM ObjectName GROUP BY field1
    ```

Remember, these are just some of the basic syntax and commonly used clauses in SOQL. SOQL is a powerful query language for retrieving data from Salesforce objects, and it offers much more functionality beyond what's listed here.

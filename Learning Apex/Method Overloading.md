# Method Overloading
Method overloading is a concept where multiple methods in a class can have the same name but different parameters.

## Here's how method overloading works in Apex:

##### Same Method Name: Overloaded methods in Apex have the same name but differ in their parameter lists (number, types, or order of parameters).

##### Return Type: Like in other languages, method overloading in Apex cannot be based solely on differences in return type. The method signatures must be different, which includes the method name and parameter list, but not the return type.

##### Parameter List Differences: The parameter lists of overloaded methods must differ in at least one of the following ways:

- The number of parameters.
- The data types of parameters.
- The order of parameters.
- Compile-Time Polymorphism: Method overloading in Apex, is an example of compile-time (static) polymorphism. The decision about which method to call is made at compile time based on the method signature.

- Examples: Here's a simple example in Apex demonstrating method overloading:

```java
  public class Calc {
    
    // Method to add two integers
    public static Integer add(Integer a, Integer b) {
        return a + b;
    }
    
    // Method to add three integers
    public static Integer add(Integer a, Integer b, Integer c) {
        return a + b + c;
    }
     // Method to add two doubles
    public static Double add(Double a, Double b) {
        return a + b;
    }
    
    // Method to concatenate two strings
    public static String concatenate(String a, String b) {
        return a + b;
    }
  }
```

In this example, the add method is overloaded three times with different parameter lists: two methods for adding integers, one method for adding doubles, and one method for concatenating strings.

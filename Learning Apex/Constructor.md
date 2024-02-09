# Constructor
***Constructor*** is a special type of method that is automatically called when an instance (object) of a class is created. Constructors are used to initialize the state of an object, typically by initializing its member variables or performing other setup tasks.

***Syntax:*** In Apex, the constructor has the same name as the class and does not have a return type (not even void). It is invoked using the new keyword when creating an object of the class.

***Default Constructor:*** If a class does not explicitly define a constructor, Apex provides a default constructor with no arguments. This default constructor initializes member variables to their default values (e.g., null for references, 0 for integers).

***Parameterized Constructor:*** You can define constructors with parameters in Apex. These constructors allow you to initialize object state using values passed as arguments when creating an object.

***Access Modifiers:*** Constructors can have access modifiers (public, private, or protected) to control their visibility and accessibility.

 - Example:
```java
public class MyClass {
    
    // Member variable
    public Integer myValue;
    
    // Default constructor
    public MyClass() {
        // Initialization logic
        myValue = 0;
    }
    
    // Parameterized constructor
    public MyClass(Integer value) {
        // Initialization logic using parameter
        myValue = value;
    }
}
```
In this example, MyClass defines two ***constructors:*** a default constructor and a parameterized constructor. Both constructors initialize the myValue member variable. 

***Constructors*** play a crucial role in initializing object state in Apex, ensuring that objects are properly initialized before they are used in the application.

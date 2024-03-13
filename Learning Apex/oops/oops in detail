# OOPS
In Apex programming language, the term "oops" typically refers to Object-Oriented Programming (OOP) concepts. Apex is a strongly typed, object-oriented programming language used by Salesforce developers to create custom functionality on the Salesforce platform. Here's an overview of how OOP concepts are implemented in Apex:

1. **Classes and Objects**: In Apex, you can define classes using the `class` keyword. Objects are instances of classes. You can create objects using the `new` keyword followed by the class name. For example:

    ```apex
    // Define a class
    public class MyClass {
        public Integer myNumber;
        public String myString;
    }

    // Create an object of MyClass
    MyClass obj = new MyClass();
    ```

2. **Encapsulation**: Apex supports encapsulation by allowing you to define access modifiers such as `public`, `private`, and `protected` for class members (variables and methods). This helps in hiding the internal state of an object and only exposing necessary functionalities.

3. **Inheritance**: Apex supports single inheritance, where a class can inherit properties and methods from another class. This is achieved using the `extends` keyword. For example:

    ```apex
    public class ParentClass {
        public void display() {
            System.debug('Parent class method');
        }
    }

    public class ChildClass extends ParentClass {
        // Inherits display() method from ParentClass
    }
    ```

4. **Polymorphism**: Apex supports polymorphism, which allows objects of different classes to be treated as objects of a common superclass. Polymorphism is achieved through method overriding. For example:

    ```apex
    public class Animal {
        public void makeSound() {
            System.debug('Animal makes a sound');
        }
    }

    public class Dog extends Animal {
        public void makeSound() {
            System.debug('Dog barks');
        }
    }
    ```

5. **Abstraction**: Abstraction allows you to hide the implementation details of methods and only expose necessary functionalities. In Apex, abstraction is typically achieved through interfaces and abstract classes.

6. **Interfaces**: Interfaces define a contract for classes to implement. They contain method signatures without method bodies. A class that implements an interface must provide concrete implementations for all the methods declared in the interface.

    ```apex
    public interface Printable {
        void print();
    }

    public class MyClass implements Printable {
        public void print() {
            System.debug('Printing...');
        }
    }
    ```

7. **Abstract Classes**: Abstract classes are similar to interfaces but can contain both method declarations and method implementations. However, abstract classes cannot be instantiated directly.

    ```apex
    public abstract class Shape {
        public abstract void draw();
    }

    public class Circle extends Shape {
        public void draw() {
            System.debug('Drawing Circle');
        }
    }
    ```

These are the fundamental Object-Oriented Programming concepts implemented in Apex, allowing developers to write modular, reusable, and maintainable code on the Salesforce platform.

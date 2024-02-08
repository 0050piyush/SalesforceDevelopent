# Anatomy of a Class

## Class
A Class is a user-defined datatype (complex-type) and acts as a blueprint for their instances.
- Constructor: Whenever you write a class, it already has a default constructor.
- State
- Behaviour

## Object
An Object is an instance of a class i.e., a class in action.

### Example
```apex
public class Demo1 {
    public void printOutput(String stringToDisplay) {
        System.debug('Display text: ' + stringToDisplay);
    }
}

Demo1 d1 = new Demo1(); // Executed in the anonymous window of the developer console
d1.printOutput('Hello World');
Output: Hello World
```
### Methods in Apex Class

   -  Reusable code snippets
   - Specific purpose
   -  Knows what comes through
   -  Knows what goes out


| Capability        | Static (Variables, Methods) | Instance (Variables, Methods) |
| ----------------- | -------------------------- | ----------------------------- |
| **Association**   | Class based                | Object based                  |
| **Replication**   | Once                       | One copy per instance         |
| **Initialization**| Class is loaded            | Instance is created           |
| **Syntax**        | `MyClass.staticMethodName();` | `MyClass m1 = new MyClass(); m1.instanceMethodName();` |

#### Example: 
```apex 
  public class Car {
	public String companyName;
    public String model;
    public Integer averageSpeed;

    public void display(){
        System.debug('Company Name of the car: ' + companyName);
        System.debug('Model of the car: ' + model);
        System.debug('Average speed of the car: ' + averageSpeed);
    }
}

    Car obj1 = new Car();                // Executed in anonymous window of developer console
    obj1.companyName = 'BMW';
    obj1.model = 'X7';
    obj1.averageSpeed = 45;
    obj1.display();
```

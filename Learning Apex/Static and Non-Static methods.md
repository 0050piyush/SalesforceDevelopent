# Static and Non-Static Methods
- A static method is a method that belongs to a class, but it does not belong to an instance of that class and this method can be called without the instance or objects of that class.

- A static method can only access static data members and static methods but cannot access non-static methods and variables.

- A non-static method can access static data members and static methods as well as non-static members and methods of another class or same class, it can also change the values of any static data member.

```java
public class StaticAndNonStaticExample {
    public void method1(){
        System.debug('this is a non static method, need to create an object to call this method');
    }
    public static void method2(){
        System.debug('this is a static method, DO NOT need to create an object it can be called directly with class name');
    }
    StaticAndNonStaticExample.method1();                             //this will give you an error as we need to create an object before executing this method

    StaticAndNonStaticExample obj = new StaticAndNonStaticExample(); //this will run without an error
    obj.method1();                                                    

    StaticAndNonStaticExample.method2();                             //this will run without an error
}
```

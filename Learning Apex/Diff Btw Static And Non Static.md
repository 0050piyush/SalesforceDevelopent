# Static and non-static variables

Static and non-static variables are both types of variables used in programming, but they have different characteristics and purposes.

1. **Static Variables:**
   - A static variable is a variable that is associated with a class, not with any particular instance of the class.
   - There is only one copy of a static variable per class, regardless of how many instances (objects) of that class are created.
   - Static variables are initialized only once, at the start of the program's execution, and they retain their values throughout the program's execution.
   - They are typically used to store values that are common to all instances of a class, such as constants or variables that need to be shared among all instances.
   - Static variables are accessed using the class name, not through an object instance.

2. **Non-Static Variables (Instance Variables):**
   - A non-static variable, also known as an instance variable, is associated with each instance (object) of a class.
   - Each object of the class has its own copy of non-static variables, and their values can vary from one object to another.
   - Non-static variables are initialized for each object separately when the object is created, and they can have different values for different objects.
   - They are typically used to store unique data for each object, such as the state or properties of that particular object.
   - Non-static variables are accessed using object references.

In summary, the main differences between static and non-static variables lie in their association with the class or instances of the class, the number of copies created, their initialization behavior, and their usage scenarios.

&rarr; Exapmle 1:
```java
public class StaticAndNonStatic {
	public integer num1;
    public static integer num2;
    
    public void increment(){
        num1 += 10;
        num2 += 10;
	}
	public void display(){
        System.debug('num1: ' +num1);
        System.debug('num2: ' +num2);
	}
      Teacher tch1 = new Teacher();
        tch1.name = 'Rose';
        tch1.age = 20;
        Teacher.schoolName = 'Frisco High School';
      
      Teacher tch2 = new Teacher();
        tch2.name = 'Mary';
        tch2.age = 25;
        Teacher.schoolName = 'Mickkeny High School';
      
      tch1.display();
      tch2.display();
}
/*  Output => Teacher Name: Rose
              Teacher Age: 20
              School Name: Mickkeny High School

              Teacher Name: Mary
              Teacher Age: 25
              School Name: Mickkeny High School
*/
```

&rarr; Exapmle 2:
```java
public class StaticAndNonStatic {
	public integer num1;
    public static integer num2;
    
    public void increment(){
        num1 += 10;
        num2 += 10;
	}
	public void display(){
        System.debug('num1: ' +num1);
        System.debug('num2: ' +num2);
	}
      StaticAndNonStatic obj1 = new StaticAndNonStatic();
        obj1.num1 = 5;
        StaticAndNonStatic.num2 = 5;
        obj1.increment();
        obj1.display();
    
      StaticAndNonStatic obj2 = new StaticAndNonStatic();
        obj2.num1 = 5;
        obj2.increment();
        obj2.display();
}

  /*  Output => num1: 15
                num2: 15
                num1: 15
                num2: 25
  */
```

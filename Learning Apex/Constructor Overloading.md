# Constructor Overloading

constructor overloading refers to the ability to define multiple constructors within a class, each with a different set of parameters. This allows developers to create objects of the class using various combinations of parameters, providing flexibility and customization.

Constructor overloading follows the same principles as method overloading, where different methods can have the same name but different parameter lists. In Apex, when multiple constructors are defined in a class, they must have different parameter lists, either in terms of the number of parameters or the data types of the parameters.

When an object of the class is instantiated, the appropriate constructor is invoked based on the arguments provided during instantiation. The constructor with the parameter list that matches the arguments is called, and its code is executed to initialize the object.

Constructor overloading is commonly used in Apex to create objects with different initial states or configurations, allowing developers to initialize objects in various ways based on their specific requirements.

``` java
public class EmployeeExample {
	string name;
    integer age, salary;
    public void display(){
        System.debug('Name '+name);
        System.debug('Age '+age);
        System.debug('Salary '+salary);
    }
    public EmployeeExample(string n, integer a){
        name = n;
        age = a;
        salary = 40000;
    }
    public EmployeeExample(string n, integer a, integer s){
        name = n;
        age = a;
        salary = s;
    }
    public EmployeeExample(){
        name = 'no argument constructor';
        age = 18;
        salary = 100000;
    }
	EmployeeExample emp1 = new EmployeeExample();
	EmployeeExample emp2 = new EmployeeExample('John', 40);
	EmployeeExample emp3 = new EmployeeExample('Marcus', 42, 210000);
	emp1.display();
	System.debug('********');
	emp2.display();
	System.debug('********');
	emp3.display();

}
```

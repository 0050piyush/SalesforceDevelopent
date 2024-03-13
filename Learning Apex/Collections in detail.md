# Collections
Apex language provides developer with three classes (Set, List, Map) that makes it easier to handle collection of objects. In a sense, these collections works somewhat like arrays except their size can change dynamically and they have more advanced behaviours and easier access methods than arrays.
## List:

<pre>
  Violet    Indigo    Blue    Green    Yellow     Orange    Red
    0          1        2       3         4          5       6  
</pre>  

Lists are used to store data in sequence. These are the widely used collections which can store primitives, user defined objects, sObjects, Apex Objects or other collection.

There are 2 main properties of lists:

- It stores data in sequential order.

- The data which it stores is non-unique or can be duplicate.

Hence use a list when the sequence of elements is important and where uniqueness of the elements are not important.

*List initialization*

```java
   List<datatype> list1 = new List<datatype>(）：
```
- Integer Example:
```java  
   List<Integer> numbers = new List<Integer>();                                       // any data type can be used here as per the requirement
   numbers.add(1);                                                                    // add is used to add any value to List
   numbers.add(1);
   numbers.add(2);
   numbers.add(3);
   System.debug('List of numbers: ' + numbers);
   output => 1 1 2 3                                                                 // duplicate values are allowed in List
```
&rarr; can also be done like this:
```java
  List<Integer> list1 = new List<Integer>{1, 1, 2, 3};
  output => 1 1 2 3   
```

- String Example:
```java
List<String> list2 = new List<String>{'I', 'am', 'feeling', 'Good'};
output => I am feeling Good
```

## List array notation

```java
List <Integer> list3 = new List<Integer>[4];
list3[0] = 20;
list3[1] = 40;
list3[2] = 60;
list3[3] = 80;
System.debug(list3);         //output => 20 40 60 80
System.debug(list3[1]);      //output => 40
```






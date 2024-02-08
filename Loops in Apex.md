####                    --------------------------------------
##                               Loops in Apex
####                    --------------------------------------
##                     5 Types of Procedural Loops in Apex:

### 1. While
### 2. do-while
### 3. if else
### 4. Switch
### 5. For

 ### While
 ####   > While (Boolean Exit Condition)


### do-while
```java
do {
  //Code Block
}While (Boolean Exit Condition)
```

```java
int i = 5;   
do { 
 i++; 
System.out.println("GfG"); 
} while (i < 10); 
```


### if else
```java
  	if (Boolean Condition) {
  	//Code Block
  	｝
  	else if (Boolean Condition2) {
  	//Code Block
  	｝
  	else {
  		//Code Block (Optional Default Condition)
  	}
```

### Switch
```java
    Switch on expression{
  
  	when valuel, value2{
  		//Code Block
  	}
  	 
  	when value3{
  		//Code Block
  	}
  
  	when value4{
  		//Code Block
  	}
  }
```

### For
```
For (Initialization; Exit Condition; Increment/Decrement) {
          //Code Block
}

For (Variable : Array or Set) {//Code Block}
For (Variable : ([Inline SOQL Query]) {//Code Block}
for(i = 1; i <= 6; i++){
          //code block
}
```
#### For loop with List
Example:
```java
List<Integer>numbers = new List<Integer>();
Integer listSize = 6;
for(integer i = 1; i<=listSize; i++){
 numbers.add(i);
}
System.debug('List of numbers ' + numbers);
output => 1 2 3 4 5 6
```

   

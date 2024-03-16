# Data Types in javascript

JavaScript supports several data types, which include:

1. **Primitive Data Types**:

    a. **Number**: Represents numeric data, including integers and floating-point numbers.
    
    ```javascript
    var age = 25;
    var pi = 3.14;
    ```

    b. **String**: Represents textual data enclosed within single ('') or double ("") quotes.
    
    ```javascript
    var name = "John Doe";
    ```

    c. **Boolean**: Represents a logical value, `true` or `false`.
    
    ```javascript
    var isAdult = true;
    ```

    d. **Undefined**: Represents a variable that has been declared but not assigned a value yet.
    
    ```javascript
    var x;
    ```

    e. **Null**: Represents the intentional absence of any value or object.
    
    ```javascript
    var y = null;
    ```

    f. **Symbol**: Represents a unique identifier, introduced in ECMAScript 6.
    
    ```javascript
    var id = Symbol('unique');
    ```

    g. **bigInt**: Here's how you can use BigInt in JavaScript:
    ```javascript
    let bigIntSum = 12345678901234567890n + 98765432109876543210n;
    console.log(bigIntSum); // Output: 111111111111111111100n
    ```
3. **Complex Data Types**:

    a. **Object**: Represents a collection of key-value pairs.
    
    ```javascript
    var person = {
        name: "John",
        age: 30,
        isStudent: false
    };
    ```

    b. **Array**: Represents a collection of elements, each identified by an index.
    
    ```javascript
    var colors = ["red", "green", "blue"];
    ```

These are the primary data types in JavaScript. It's worth noting that JavaScript is a loosely typed language, meaning variables can hold values of any data type, and data types are automatically converted as needed during operations.

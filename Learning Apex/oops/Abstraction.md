# Abstraction

```java
abstract class Shape {
    abstract void drawShape();
    abstract integer perimeter();
    abstract integer area();

    void func() {
        System.debug('This is example');
    }
    // 1. abstract methods need no implementation
    // 2. When some class extends this, that class must override/implement these methods
    // 3. You can have normal methods also
}

class Rectangle extends Shape {
    integer length;
    integer breadth;

    public void drawShape() {
        System.debug('Drawing rectangle');
    }

    public integer perimeter() {
        return 2*(length+breadth);
    }

    public integer area() {
        return length*breadth;
    }
}

class Square extends Shape {
    integer side;

    public void drawShape() {
        System.debug('Drawing square');
    }

    public integer perimeter() {
        return 4*side;
    }

    public integer area() {
        return side*side;
    }
}

public class Abstraction {
    public static void main() {

    }
}
```

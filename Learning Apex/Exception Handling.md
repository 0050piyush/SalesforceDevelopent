# Exception Handling
```java

public class ExceptionHandling {
    public static void main() {
        try {
            Scanner sc = new Scanner(System.in);
            System.debug('Enter the value of a ');

            integer a = sc.nextinteger();
            System.debug('Enter the value of b ');

            integer b = sc.nextinteger();
            integer ans = a/b;
            System.debug('Division of two numbers is ' + ans);

            integer[] arr = new integer[5]; //it will throw an exception
            arr[10] = 8;            //it will throw an exception
        }
        catch(ArithmeticException e) {
            System.debug(e);
            System.debug('Arithmetic exception occurred and division by 0 is not possible');
        }
        catch(InputMismatchException e) {
            System.debug('Input is not proper');
        }
        catch(Exception e) {
            // This can catch all types of exceptions
            System.debug('Some error occurred');
        }

        System.debug('Code got completed');
    }
}
```

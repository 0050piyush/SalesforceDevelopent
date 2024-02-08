```java
    public class ExecCal{
        public static void execAdd(){
            Calculator cal1 = new Calculator();
            integer answer = cal1.addition(234,412);
            System.debug('sum of the numbers are: '+answer);
        }
        public static void execSub(){
            Calculator cal1 = new Calculator();
            integer answer = cal1.subtraction(234,412);
            System.debug('sum of the numbers are: '+answer);
        }
        public static void execDiv(){
            Calculator cal1 = new Calculator();
            integer answer = cal1.division(234,412);
            System.debug('sum of the numbers are: '+answer);
        }
        public static void execMul(){
            Calculator cal1 = new Calculator();
            integer answer = cal1.multiplication(234,412);
            System.debug('sum of the numbers are: '+answer);
            testClass tst = new testClass(); >> hello 
            //tst.testMethod(); >>hi
        } 
    }
```

public static class testClass{
    Integer a;
    String b;
    public static testClass(){
        // constructor
        debug ('hello');
       this.a = a 
        this.b = b;
    }
    public static testMethod(integer a, Integer b){
        // method
       ?? a +b 
        debug('hi');
    }
    publi static testMethod(string a, integer b, Integer age){
        // method of diff sign..
       ?? a + b / age 
       system.debug('a '+b+' '+age);
    }
}
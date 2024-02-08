# Creating a calculator Using a Simple Method
- Example:
```java
        public class Calculator {
        	integer num1, num2,result;
            
            public integer addition (integer a, integer b){
                result = a+b;
                return result;
            }
            
            public integer subtraction (integer a, integer b){
                if(a>b){
                    result = a-b;
                }else{
                    result = b-a;
                }
                
                return result;
            }
            
            public integer multiplication (integer a, integer b){
                result = a*b;
                return result;
            }
            
            public integer division (integer a, integer b){
                if(a>b){
                    result = a/b;
                }else{
                    result = b/a;
                }
                
                return result;
            }
        
          Calculator cal1 = new Calculator();
          
          integer answer = cal1.addition(234,412);
          System.debug('sum of the numbers are: '+answer);
          
          integer answer1 = cal1.subtraction(43532,2345);
          System.debug('subtraction of the numbers are: '+answer1);
          
          integer answer2 = cal1.subtraction(655,2134);
          System.debug('subtraction of the numbers are: '+answer2);
          
          integer answer3 = cal1.multiplication(328,23);
          System.debug('Multiplication of the numbers are: '+answer3);
          
          integer answer4 = cal1.division(6556,53);
          System.debug('Division of the numbers are: '+answer4);
        
        }
```


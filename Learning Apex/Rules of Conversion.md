# Rules of conversion:

In general, apex requires explicit conversion from one datatype to another however a few datatype can be implicitly converted like variables of lower numeric type to higher types.

Hierarchy of Data Types: integer<long<double<decimal

### if you want to store an integer value in a double you can use typecast for that:

- example: double d = 2.355;
           integer i = d;                   // it will throw a compile time error
           integer i = (integer)d;          // it will work

**Note:** Once a value has been passed from a number of lower type to a number of higher type, the value is converted to the higher type of number.

&rarr; Ids can always be assigned to strings.

&rarr; String can be assigned to ids however at runtime the value is checked to ensure that it is a legitimate id, if it is not then a runtime error is thrown.

&rarr; If the numeric value of the right hand side exceeds the maximum value for an integer you get a compilation error. In this case, the solution is to append L or I to the numeric value so that it represents a long value which has a wider range.

&rarr; Arithmetic computation that produce values larger than the max values of the current type are set to overflow.

Ex: Integer i= 2147483647 + 1; // overflow



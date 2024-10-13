Floating point numbers are represented using multiple parts, the ==exponent== and the ==mantissa==


to store numbers with a fractional component, the number line extends powers of 2 beyond 0
2<sup>3</sup>   2<sup>2</sup>   2<sup>1</sup>   2<sup>0</sup>   2<sup>-1</sup>   2<sup>-2</sup>   2<sup>-3</sup> 
8     4     2     1    $\frac12$     $\frac14$     $\frac18$

so a number 0110 1100 would be 2<sup>3</sup> + 2<sup>2</sup> + 2<sup>0</sup> + 2<sup>-1</sup> 
8 + 4 + 1 + $\frac12$ = 13.5

this works for fixed point numbers, where the accuracy of the number is a fixed amount ie. certain number of decimal places

to increase accuracy / have more decimal places, the bit values can be shifted by a power of 2

so 
-32 16 8 4 2 1  $\frac12$ $\frac14$ 
 becomes
 -8 4 3 2 1 $\frac12$ $\frac14$ $\frac18$ 

To do this, the binary data must be split into two parts:
- mantissa - the binary values above
- exponent - **how much the values in the mantissa are shifted by**

## exponent / mantissa

in a single byte, the exponent takes up 3 bits and the mantissa takes up 5 bits

==exponent==        ==mantissa==         
-4  2  1             -1 $\frac12$ $\frac 14$ $\frac 18$ $\frac 1{16}$      
 0  0  1              1  0  1  1  1

the two's compliment number in the exponent tells you how many times the values are shifted

a value of 1 (001) in the exponent multiplies all the bit values in the mantissa by 2<sup>1</sup>  - equivalent to a single shift left

similarly, a value of -4 (100) in the exponent multiplies all the bit values by 2<sup>-4</sup> - equivalent to 4 shifts right

the exponent has a sign bit, so the mantissa values can be shifted left or right

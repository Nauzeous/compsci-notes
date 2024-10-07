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
signed numbers are numbers that can be negative, and the range of numbers is spread evenly across positive and negative

there is multiple ways to represent signed numbers in binary, but two's complement is the best

-4  -  1 1 0 0
-3  -  1 1 0 1 
-2  -  1 1 1 0
-1  -  1 1 1 1
0  -  0 0 0 0
1  -  0 0 0 1
2  -  0 0 1 0
3  -  0 0 1 1

a sign bit is used at the start of the value, to determine if the number is negative or positive

if the first bit is 1, the number is negative and the number starts at a negative number, and the rest of the numbers are added.

to turn a number into it's negative version, flip the value of all bits, then add one

ie.
4 is
0 1 0 0 
flip the bits and it becomes
1 0 1 1
then add one to get negative 4 
1 1 0 0

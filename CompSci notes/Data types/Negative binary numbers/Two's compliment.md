signed numbers are numbers that can be negative, and the range of numbers is spread evenly across positive and negative

there is multiple ways to represent signed numbers in binary, but 2s compliment is preferred

-4  -  1 1 0 0
-3  -  1 1 0 1 
-2  -  1 1 1 0
-1  -  1 1 1 1
0  -  0 0 0 0
1  -  0 0 0 1
2  -  0 0 1 0
3  -  0 0 1 1

a sign bit is used at the start of the value at the **Most Significant Bit,** to determine if the number is negative or positive

if the first bit is 1, the number is negative and the number starts at a negative number, and the number is counted backwards from the lowest negative value

to express the number -12 in 8 bit 2s compliment

| -128 | 64  | 32  | 16  | 8   | 4   | 2   | 1   |
| ---- | --- | --- | --- | --- | --- | --- | --- |
| 1    | 1   | 1   | 1   | 0   | 1   | 0   | 0   |

$(-128) + 64 + 32 + 16 + 4 = 12$ 

to turn a number into it's negative version, and vice versa, flip the value of all bits, then add one

ie.
4 is
0 1 0 0 
flip the bits and it becomes
1 0 1 1
then add one to get negative 4 
1 1 0 0

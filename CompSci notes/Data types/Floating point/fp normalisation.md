By using floating point representation, it is possible to represent the number 1 in an infinite number of ways, limited only by the number of bits

ie. 
01000 001 is $\frac12$ shifted left once
00100  010  is $\frac 14$ shifted left twice
00010 011 is $\frac18$ shifted left three times

to make storage of floating point numbers consistent, normalisation is used, so the largest value in the mantissa is an exponent of $\frac12$ 

example: 
6.8
4 + 2 + 0.5 + 0.25 + 0.03125 + 0.015625= 6.78125 ()

| exponent |     |     | mantissa |           |           |           |              |              |
| -------- | --- | --- | -------- | --------- | --------- | --------- | ------------ | ------------ |
| -4       | 2   | 1   | -1       | $\frac12$ | $\frac14$ | $\frac18$ | $\frac1{16}$ | $\frac1{32}$ |
| 0        | 1   | 1   | 0        | 1         | 1         | 0         | 0            | 1            |
 
in the example, this would be the first, $\frac12$ shifted left once - 01000 001

not only does normalisation make floating point numbers more consistent, it also ensures that they are being represented with the highest possible accuracy

## Identify normalised fp numbers

all positive normalised numbers start with 01
all negative normalised numbers start with 10

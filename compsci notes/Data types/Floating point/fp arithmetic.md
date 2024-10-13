adding two normalised floating point numbers is similar to regular binary addition

however, before performing bit addition, the numbers must account for the bit shift done by the exponent

both numbers are bit shifted by their mantissa, then added together like regular integer binary

example:
5 + 1.375
## Number 1

| Exponent |     |     | Mantissa |           |           |           |              |
| -------- | --- | --- | -------- | --------- | --------- | --------- | ------------ |
| -4       | 2   | 1   | -1       | $\frac12$ | $\frac14$ | $\frac18$ | $\frac1{16}$ |
| 0        | 1   | 1   | 0        | 1         | 0         | 1         | 0            |
$(0.5+ 0.125) * 2^3 = 5$
## Number 2
| Exponent |     |     | Mantissa |           |           |           |              |
| -------- | --- | --- | -------- | --------- | --------- | --------- | ------------ |
| -4       | 2   | 1   | -1       | $\frac12$ | $\frac14$ | $\frac18$ | $\frac1{16}$ |
| 0        | 0   | 1   | 0        | 1         | 0         | 1         | 1            |
|          |     |     |          |           |           |           |              |
$(0.5 + 0.125 + 0.0625) * 2^1 = 1.25$

to add the two numbers by hand, line up their "decimal points" on a fixed point table

| values   | -16 | 8   | 4   | 2   | 1   | $\frac12$ | $\frac14$ | $\frac18$ |
| -------- | --- | --- | --- | --- | --- | --------- | --------- | --------- |
| number 1 | 0   | 0   | 1   | 0   | 1   | 0         | 0         | 0         |
| number 2 | 0   | 0   | 0   | 0   | 1   | 0         | 1         | 1         |
| result   | 0   | 0   | 1   | 1   | 0   | 0         | 1         | 1         |
the result is 4 + 2 + 0.25 + 0.125 = 6.375
the result is then [[fp normalisation|normalised]]
(more bits have been added for accuracy)

| exponent |     |     | mantissa |           |           |           |              |              |              |
| -------- | --- | --- | -------- | --------- | --------- | --------- | ------------ | ------------ | ------------ |
| -4       | 2   | 1   | -1       | $\frac12$ | $\frac14$ | $\frac18$ | $\frac1{16}$ | $\frac1{32}$ | $\frac1{64}$ |
| 0        | 1   | 1   | 0        | 1         | 1         | 0         | 0            | 1            | 1            |
## Binary subtraction

subtraction is similar to addition, but the number to be subtracted is turned negative using [[Two's compliment]] (flip all bits and add 1)

example 2:
 4 - 3.75

| exponent |     |     | mantissa |           |           |           |              |
| -------- | --- | --- | -------- | --------- | --------- | --------- | ------------ |
| -4       | 2   | 1   | -1       | $\frac12$ | $\frac14$ | $\frac18$ | $\frac1{16}$ |
| 0        | 1   | 1   | 0        | 1         | 0         | 0         | 0            |
$0.5 * 2^3 = 4$

| exponent |     |     | mantissa |           |           |           |              |
| -------- | --- | --- | -------- | --------- | --------- | --------- | ------------ |
| -4       | 2   | 1   | -1       | $\frac12$ | $\frac14$ | $\frac18$ | $\frac1{16}$ |
| 0        | 1   | 0   | 0        | 1         | 1         | 1         | 1            |
$(0.5 + 0.25 + 0.125 + 0.0625) * 2^2 = 3.75$

put 4 and 3.75 into table

| Values   | -8  | 4   | 2   | 1   | $\frac12$ | $\frac14$ | $\frac18$ |
| -------- | --- | --- | --- | --- | --------- | --------- | --------- |
| number 1 | 0   | 1   | 0   | 0   | 0         | 0         | 0         |
| number 2 | 0   | 0   | 1   | 1   | 1         | 1         | 0         |
turn 3.75 negative, transforming the operation from $4 - 3.75$ into $4 + (-3.75)$

| Values   | -8  | 4   | 2   | 1   | $\frac12$ | $\frac14$ | $\frac18$ |
| -------- | --- | --- | --- | --- | --------- | --------- | --------- |
| number 1 | 0   | 1   | 0   | 0   | 0         | 0         | 0         |
| number 2 | 1   | 1   | 0   | 0   | 0         | 1         | 0         |
| result   | 0   | 0   | 0   | 0   | 0         | 1         | 0         |
result is 0.25

then normalise result

| exponent |     |     | mantissa |           |           |           |              |
| -------- | --- | --- | -------- | --------- | --------- | --------- | ------------ |
| -4       | 2   | 1   | -1       | $\frac12$ | $\frac14$ | $\frac18$ | $\frac1{16}$ |
| 1        | 1   | 1   | 0        | 1         | 0         | 0         | 0            |


An array is a data structure that can contain multiple data items

This is done by allocating a chain of memory locations for the purpose of storing the data in the array

lists are slightly different to arrays as lists are not contiguous (the memory locations are not in a chain, one after another)

## Indexing

Once the program knows the position in memory where the array starts, another index is created, relative to the start position

| Address | ==65== | 66  | 67  | 68  | 69  | 70  |
| ------- | ------ | --- | --- | --- | --- | --- |
| value   | ==A==  | B   | C   | D   | E   | F   |
the start position of the array is stored as 65, and when a piece of data is requested with an index, the index is added to the start position

index = 2

| Address | 65  | 66  | ==67== | 68  | 69  | 70  |
| ------- | --- | --- | ------ | --- | --- | --- |
| value   | A   | B   | ==C==  | D   | E   | F   |

## Array dimensions

The number of dimensions of an array is decided by how many times a list is stored within a list

A 1-dimensional list is linear:

| Angola | Austria | Belgium |
| ------ | ------- | ------- |

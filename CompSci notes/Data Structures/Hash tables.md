The goal of a hash table is to immediately find an item in a sorted/unsorted list **without having to compare** other items in the data set

programming languages use hash tables to implement dictionaries

[[Hashing]] is used to determine the position of an item in a hash table

the hashing function is run on an item to determine the hash value, which decides its position in the hash table

there is usually a compromise between efficiency of the algorithm and the size of the hash table

A good hashing function should:
- be computationally cheap (quick and memory efficient)
- result in as few collisions as possible

## Resolving hash collisions

a ==hash collision== occurs when two data items have the same hash value

Although good hashing algorithms will very rarely produce clashing hash values from different inputs, it is still a possibility and must be accounted for

one method of hash collision resolution is repeatedly checking the next available space in the hash table until an empty position is found, where the value is stored

to find the item, the hashing function will give the index of the first item with the value, then linearly search through the hash table until the item is found

this is called ==linear probing==

linear probing could prevent other items from being stored in their correct location in the hash table

it could also result in **clustering**, where positions are mostly filled around common collision values

the second method of handling collisions is using a **two dimensional hash table**

this makes it possible to store multiple items in the same position (AKA ==chaining==)

another method is using a second table for collisions, called an ==overflow table==

a **linked list** could be used to implement an overflow table

## Uses

hash tables can be used in situations where items in large data set need to be found quickly, such as:
- file systems searching for a file
- identifying keywords in a programming language during compilation

## Operations

- add - add an item to the hash table
- delete - delete an item from the hash table
- retrieve - retrieve a value from the hash table using its hash value
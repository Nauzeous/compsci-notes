==An array is a data type that can hold multiple data items==

this is done by allocating a **contiguous** (consecutive) chain of memory

the difference between lists and arrays is that they are **not contiguous** in memory

==lists can support heterogenous data, while arrays are homogenous==

The start position of the array is stored as the address

| ==65== | A   |
| ------ | --- |
| 66     | B   |
| 67     | C   |
| 68     | D   |
| 69     | E   |
to access individual items, another index (relative to the start address) is used

for example, if the start is 65, and i want to access the third item, i get the item in memory at address 65 + 3, which is D

| 65     | A   |
| ------ | --- |
| 66     | B   |
| 67     | C   |
| ==68== | D   |
| 69     | E   |
This type of list is also called one dimensional, as it contains single items, and not other lists

A 2-dimensional array would look similar

| ==65== | A   | a   |
| ------ | --- | --- |
| 66     | B   | b   |
| 67     | C   | c   |
| 68     | D   | d   |
| 69     | E   | e   |
to access an item in the 2d array, two indexes are required

the start position is known, so the first index controls which row 

eg. \[2]\[1]

65 + 2 = 67

| 65     | A     | a     |
| ------ | ----- | ----- |
| 66     | B     | b     |
| ==67== | ==C== | ==c== |
| 68     | D     | d     |
| 69     | E     | e     |
0 + 1 = 1

| 0   | 1     |
| --- | ----- |
| C   | ==c== |
the selected item  is "c"

by using lists inside lists / arrays inside arrays, any dimensional array is possible

## Records

a record data structure is a collection of related fields, where each field is a variable

each field in a record can hold any type of data


##  Car

| Reg_plate | Make   | Model   | Price | Engine_size | Petrol |
| --------- | ------ | ------- | ----- | ----------- | ------ |
| HG26LOP   | Toyota | Corolla | 17000 | 1.8         | True   |
The **Car** record can be used to make many different types of car, although only 1 example was shown

The record data structure is similar to a class, except immutable and without class 
methods

## Lists vs arrays vs tuples

**Lists**:
-  [x]  Mutable 
-  [x] Can support multiple data types
-    Python syntax - *list* / \[   ]

**Arrays**:
-  [x]  Mutable 
-  [ ] Can support multiple data types
-    Python syntax - same as list

**Tuple**:
-  [ ]  Mutable 
-  [x] Can support multiple data types
-    Python syntax - *tuple* / (   )



merge sort sorts data quickly using a divide and conquer method

the merge sort repeatedly halves the data set until each item is its own list

then each item is merged together in order


eg.
```
 [9,8,7,6,5,4,3,2,1]

 [9,8,7,6] [5,4,3,2,1]

 [9,8] [7,6] [5,4] [3,2,1]

 [9] [8] [7] [6] [5] [4] [3] [2] [1]
 
 [8,9] [6,7] [4,5] [2,3] [1]

 [6,7,8,9] [4,5] [1,2,3]
 
 [6,7,8,9] [1,2,3,4,5]

 [1,2,3,4,5,6,7,8,9]
```

merge sort is suitable for any data set but works best with large data sets and when memory usage is not limiting

it is suited to parallel processing as it operates on a divide and conquer basis

1. repeatedly divide the list into halves until each item is its own list
2. take two adjacent lists and start with the first item in each one
3. compare the two items
4. insert the lowest item into a new list, move to the next item in the list it was taken from
5. repeat 3 and 4 until all the items from one of the lists are in the new list
6. append all the items from the list that still contains items to the new list
7. replace two adjacent lists with new longer list
8. repeat 2-7 until all adjacent lists are compared
9. repeat 2-8 until there is 1 list


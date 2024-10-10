the binary search is an efficient algorithm for searching a sorted data set

it works by using a divide and conquer strategy:

start at the middle, if the target item is larger than the middle, then the entire lower half can be discarded and vice versa

by repeating this pattern, the list will be continually halved until there is only 1 item left, or the target item is the middle item

if the final item is not the target item, then the item is not in the list

as the algorithm halves the list with each pass, it makes the average time complexity and the worst time complexity $O(\log_2{n})$

a binary search implementation would look like:

```
found = False
first = 0
last = items.length-1
while first <= last:
	middle = (first + last) // 2
	if items[middle] == target_item:
		found = True
		break
	elif items[middle] < target_item:
		first = midpoint + 1
	else:
		last = midpoint - 1

```


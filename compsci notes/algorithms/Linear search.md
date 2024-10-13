a linear search starts with the first item in a list and checking each item one by one, until it gets to the end.

a linear search doesn't require a sorted list of data, but is slow in large data sets, taking $O(n)$ time

an implementation would look like

```
found = False
i = 0
while i < items.length:
	item = items[i]
	if item == item_to_find:
		found = True
		break
	i = i + 1
```

if the loop finishes and the found variable is still False, then the item was not found in the list









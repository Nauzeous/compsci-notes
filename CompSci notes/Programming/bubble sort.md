bubble sort orders an unordered list by comparing each item with the next one and swapping them if they are out of order

this effectively "bubbles" the Nth largest item to the top with the Nth pass

```
length = len(items)
swapped = True
while length > 0 and swapped:
swapped = False
length=length-1
for i in range(length):
	if items[i] > items[i+1]:
		swap(items[i],items[i+1])
		swapped = True
```

the swapped variable is a *bool* that tracks whether any items have been swapped during the pass

if no items are swapped, then the list is sorted, so the program ends

as a fail safe, the program also stops if the number of passes exceeds the length of the list

with each pass, you only need to bubble up to 1 less than the previous pass, as the nth largest item will be at the position (length-n), and will be sorted already

the inner for loop is a single pass

swap is treated as a black box for the spec
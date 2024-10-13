when comparing the performance speed of algorithms, the complexity of the algorithm is key

ideally, an algorithm runs quickly and takes up minimal space

the time complexity is a function that determines how the time taken to complete an algorithm changes with the scale of input

the function is not to be taken too literally, and is just an indicator of how well an algorithm performs at a large scale

for example, take a program that sums all the numbers from 1 to *N*

this can be implemented as
```
def sumIntegers(n):
	sum = 0
	for i in range(n+1):
		sum = sum + i
	return sum
```

since this algorithm has a for loop that has a number of iterations proportional to *N*, the time complexity is $\mathcal{O}(n)$ 

with a smarter implementation 
```
def sumIntegers(n):
	sum = n * (n+1) / 2
	return sum
```
this version does not use a for loop, so the amount of lines that the function executes is independent of N, thus the time complexity is $\mathcal{O}(1)$ which means the time complexity is *constant*

as well as time complexity, there is space complexity, which works on the same principles but instead measures the amount of memory that is used by a program

[[Algorithm complexity|time complexity for each search algorithm]]




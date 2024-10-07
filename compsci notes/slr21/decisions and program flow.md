decisions can affect program flow as they choose which code is executed

the code that is executed inside the branch of the decision should be unique to the branch, ie. code should not be repeated

eg.

```
y = int(input())
x = 2

if y>3:
	x = x + 2
	print(x)
else:
	x = x - 2
	print(x)
```

can be written as

```
y = int(input())
x = w

if y > 3:
	x = x + 2
else:
	x = x - 2

print(x)
```
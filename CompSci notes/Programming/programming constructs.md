### sequence

sequence is the default programming construct, involving executing instructions one after another

purely sequence programs would be deterministic, thus not very useful

### selection

selection is a construct that allows a program to change direction (branch) based on a boolean expression

the most common selection statement is *if*, often used with *else*

```
if x:
	...
else:
	...
```
### iteration

there are multiple ways to iterate over sections of code, but the most common is a for loop

count controlled loops are used when the required number of iterations is known before entering the loop

```
for i in range(10):
	x = x * i
```

condition-controlled loops are also important, as they can be used when the required number of iterations is not known because the condition changes within the loop 

```
while inp != answer:
	inp = input("...")
```

you can also nest constructs inside each other; if and for can be used within each other etc.

```
for i in range(8):
	if i % 2 == 0:
```


however, overly nesting code is almost never needed, and should be avoided to keep code readable 



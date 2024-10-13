A local variable has scope within a function

a global variable can be accessed from anywhere in the program

```
def foo():
	x = 10
	for i in range(4):
		x += 1
		print(x)
	return

x = 2
foo()
print(x)
```

returns 10 11 12 13 2
### local
- accessible single subroutine
- created inside a subroutine
- destroyed when the subroutine exits

### global
- accessed throughout the program
- created outside a subroutine at the start of the program
- destroyed when the program ends


global variables should only be used where necessary


global variables make programs harder to maintain, as it makes them harder to test, debug, and maintain

as such they are considered as poor programming practice

although there are situoations where using one is necessary

it is better to pass values by parameters

there are variable levels of scope, although higher level languages do not provide as much control

eg. extern, static, 


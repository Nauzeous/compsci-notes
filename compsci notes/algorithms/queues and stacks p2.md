[[Stacks and queues]]

there are different ways of implementing stacks and queues, as all they need to do is basic operations

for stacks:
- push
- pop
- peek
for queues:
- enqueue
- dequeue
- peek

one way of implementing a stack is with a static array and a pointer to the last item, (top pointer) that is incremented when something is pushed onto the stack and decremented when something is popped off the stack

```
class Stack:
	def __init__(self,maxsize):
		self.items = [0 for i in range(maxsize)]
		self.maxsize = maxsize
		self.toppointer = -1

	def push(self,item):
		if self.toppointer == self.maxsize:
			return
		self.toppointer += 1

		self.items[self.toppointer] = item

	def pop(self):
		if self.toppointer == -1:
			return
		poppeditem = self.items[self.toppointer]
		self.items[self.toppointer] = 0
		self.toppointer -= 1
		return poppeditem

	def peek(self):
		return self.items[self.toppointer]
```

queues also have some variance in the way they are implemented, as they can be circular (loops back to start when queue length is exceeded)
```
frontptr = (frontptr + 1) % maxsize
```
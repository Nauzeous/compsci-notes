
Stacks are ==last-in first-out== data structures, meaning that the only item that can be popped off is the item on the end of the stack (last item pushed to stack)

Stacks are implemented using arrays but can be done by using a class object

Processors use stacks to track the flow of programs

when a procedure/subroutine is called, it changes the value of the program counter to the first instruction of the subroutine

When the subroutine ends, the processor returns the program counter to the previous value, which is stored on a stack, allowing subroutine calls to be nested

local variables are also held on the stack, which makes them local: once the subroutines ends,the local variables are popped off the stack

Interrupts are also handled with a stack, and must have a way of determining if they are full 

Stacks are used for:
- performing depth-first searches on graph structures
- keeping track of user inputs (ie. delete) in case the user wants to undo
- backtracking algorithms (pathfinding)
- evaluating mathematical expressions

Operations that can be performed on a stack:
- push: add an item to the end of the stack
- pop: remove last item from the stack
- peek: return item from end of stack (without removing it)

## Queue

A queue is a linear data structure, where items can be queued and dequeued from the front of the queue

items are usually popped off the front of the queue, but it is possible to jump the queue, by using a priority queue

new items can also join at the front of the queue, although they usually join from the end

Queues are ==first-in first-out==, using a back pointer that points to the last item in the queue, called a tail pointer

queues also have front pointers that point to the first item

queues can be implemented using arrays and class objects, similar to stacks

Queues are used for:
- process scheduling
- transferring data between processors
- performing breadth-first searches on graph structures


operations that can be performed on a queue:
- Enqueue - add an item to the end of the queue
- dequeue - remove item from the front of the queue
- peek - return the value from the front of the queue (without removing it)
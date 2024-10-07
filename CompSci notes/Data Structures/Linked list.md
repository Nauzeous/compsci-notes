A linked list is a data structure that is used to build other data structures like:
- [[Stacks and queues|Stacks]]
- [[Stacks and queues|Queues]]
- graphs
- trees

Linked lists are constructed from nodes and pointers

| Index   | 0   | 1   | 2   | 3   | 4   | 5    |
| ------- | --- | --- | --- | --- | --- | ---- |
| data    | A   | a   | B   | b   | C   | c    |
| pointer | 2   | 3   | 4   | 5   | 1   | null |

traversing the list would give "ABCabc"

the list **ends with a null pointer**

A start pointer identifiies the starting node

Each node contains data and a pointer to the next node, so each item links to another address in the list

**this allows programming languages to support lists**, as pointers can point to any memory address, so any size item can fit in the list

By adding an extra pointer, nodes can point to the previous item, along with the next, this creates a ==doubly linked list==

if the last pointer in a linked list links to the first node, it is called a ==circular linked list==

## implementation


although linked lists can be implemented with contiguous, static arrays, they are better with an object-oriented approach, similar to many other data structures

in a linked list using objects, any available memory address can be used to store data

the memory footprint of the data structure is not determined at compile time and can dynamically change at runtime, meaning linked lists are a dynamic data structure

## Applications

Linked lists are used for:
- operating systems managing a processor to store process blocks in a ready state
- image viewers to switch between previous and next images
- music players storing songs in a playlist
- web browsers navigating through links
- collision resolution in hash tables
- maintaining drives file allocation tables

## Operations

the operations that can be performed on a linked list:
- **Add** - add a new node
- **delete** - removes a node
- **next** - moves to the next node
- **previous** - moves to the previous node (doubly linked lists only)
- **traverse** - linear search the list

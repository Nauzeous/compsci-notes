A tree is a fundamental data structure, made of nodes and pointers

each tree has a root at the top , with branches coming off, connecting to multiple child nodes

the nodes at the bottom of the tree are called leaf nodes

A set of nodes and edges from a single node through all the descendants is called a ==subtree==

Trees are used for:
- file management with folders
- pathfinding algorithms like A*
- storing and manipulating hierarchical data ie. family tree

## Binary trees

binary trees are a subset of trees, that are limited in how many child nodes a parent node can have, ==up to two==.

Binary trees can be represented with dictionaries, similar to graphs

as the maximum number of child nodes is fixed, they can also be stored as a two dimensional array (empty pointers are stored as *null*)

However, it is more common to represent binary trees with objects

Binary trees are used for:
- database searching and sorting
- networks and router tables
- OS scheduling processes
- huffman coding for compression
- cryptography
## Operations

- add - add a new node to the tree
- remove - remove a node from the tree
- Binary search - returns data stored in a node
- pre-order [[tree operations|traversal]]
- in-order traversal
- post-order traversal
- breadth first search
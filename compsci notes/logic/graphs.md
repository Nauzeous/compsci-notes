==A graph is a data structure made of nodes and pointers== (vertices and edges in a mathematical context)

graphs are different from linked lists and binary trees because ==each vertex can have more than two edges==

edges can point in a specified direction (**directed graph**) or no direction (**undirected graph**)

==graphs can also be weighted==, giving each edge a value ie. distance or some sort of cost (used in dijkstra's algorithm)

a graph is represented in code with a dictionary

python syntax:

graph = \["A":\["B","C","D"],"B":\["A","C",E"],"C":\["A","B","D"],"D":\["A","C","F"],"E":\["B"],"F":\["D"]]

a weighted graph is represented similarly

graph = \["A":\["B":19,"C":17,"D":21],"B":\["A":19,"C":11,"E":12],"C":\["A":17,"B":11,"D":9],"D":\["A":21,"C":9,"F":10],"E":\["B":12],"F":\["D":10]]

the dictionary used to represent graphs is called an ==adjacency list==, but they can also be stored by an ==adjacency matrix==, with rows and columns representing which nodes connect to other nodes with a 1

graphs are used for:
- mapping road networks
- storing data in databases
- resource allocation in operating systems
- representing molecular structures

# Operations on graphs

Standard operations:
- Adjacent - return whether there is an edge connecting two nodes
- Neighbours - return all nodes connected to a node
- Add - add a new node
- Remove - remove a node
- Add edge - add a new edge
- Remove edge - removes an edge
- get node value - return value in a node
- set node value - set value in a node
- get edge value - return value of an edge
- set edge value - set value of an edge

Search operations:
- depth-first search - explores each branch fully before backtracking
- breadth-first search - explores each neighbouring node before moving to vertices at the next depth

[[tree operations|traversal operations]]:
- pre-order traversal
- in-order traversal
- post-order traversal


[[graphdiagram.excalidraw]]
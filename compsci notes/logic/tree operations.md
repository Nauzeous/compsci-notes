multiple types of operations, beyond normal operations with basic functionality, there is searching/traversing

## Depth-first

implemented using a stack

pre-order:
[[traversal.excalidraw|diagram]]
- can be done recursively easily using the instructions {output current node, traverse left, then traverse right}
in-order:
- done recursively with the instructions {traverse left, output current node, traverse right}
post-order:
- done recursively with the instructions {traverse left, traverse right, output current node}


## Breadth-first

implemented using a queue
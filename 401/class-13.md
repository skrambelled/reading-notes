# Trees

Trees are a data structure where 1 node can point to multiple nodes.

Your file system can be thought of as a tree. Where each folder is a node and may have multiple files and folders which are themselves nodes.

Some Trees are binary trees, where each node can point to two additional nodes.

Traversing these trees are often done by recursion, where in the recurive call the root of the tree is defined as a node, and its children are the leaves. On the next recursive call, a leaf would be defined as the root. Through this recursion we can traverse through a whole Tree system, binary or otherwise.

Three methods of depth-first traversal using the call stack:

1. Pre-order (output value -> look left -> look right)
2. In-Order (look left -> output value -> look rght)
3. Post-order (look left -> look right -> output value)

Breadth first traversal using a queue:

1. enqueue node, enqueue left, enqueue right

[<-- Back](../README.md)

# Linked lists

Linked lists are a series of nodes, where each node can point to the next one.

A singly linked list has nodes that only point in one direction:

A -> B -> C -> etc

A doubly linked list points both forwards and backwards:

A <-> B <-> C <-> etc

The *head* is the first node in the series, and the *current* is the node we are currently on. Typically, when you are done using a linked list you will reset the current back to the head, so that you can start back overt at the beginning.

*next* points to the next node. You can traverse a node by referring to this next pointer in a `while` loop. When you read the last node in the list, next will be `null`.

There are lots of useful ways to manipulate linked lists. For example, if you adding a node to the beginning, you can simply point the head to this new node, and set that node's next pointer to the original head.

If you are inserting a node somewhere else, you can point the prior node to the new one, and point the new node to the prior's next.

Unlike some contiguous data structures, linked listed are allocatated dynamically because nodes point to one another. We know where were are in a linked list because we're traversing through these pointers rather than using some index value. This means a linked list can grow and shrink relatively inexpensively.

Its still often preferred to use a traditional array (or list). You cannot search through a linked list as fast as you can through a sorted array, because you cannot binary search through a linked list. It can be better for dynamically adding nodes though.

[<-- Back](../README.md)

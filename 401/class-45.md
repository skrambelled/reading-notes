# Graphs

A graph is a non-linear data structute, comprised of vertices (or nodes) that are interconnected.

Key terms:

- Vertex - or a node
- Edge - a connection between nodes
- Neighbor - adjacent node, or a node connect to another by an edge
- Degree - number of edges that a given node has

## Undirected and Directed Graphs

A graph with no direction, where the edges are bi-directional is undirected.

Sometimes an edge only travels in one direction, and if every edge in a Graph does so, it is a directed Graph.

## Complete vs Connectecd vs Disconnected

A complete Graph is when every node is connected to every single other node

A connected Graph is when all nodes have at least one edge, and are connected in one 'clump'

A disconnected Graph will have multiple islands of nodes, and sometimes even completely isolated node.

## Acyclic vs Cyclic

An acyclic Graph is one without cycles, like a Tree

A cyclic Graph has cyclese, Like a Circularly Linked List

## Adjecency Matrix

An adjecency matrix has every node on both the x and y axis, and then a 1 to represent when a node is connected by an edge to another node. When notating a Undirected Graph in this manner, it will always be symmetric because when Node A is connected to Node B, Node B is also connectr to Node A. When representing a Directed Graph with an adjacency matrix, it may not be symmetric.

## Adjacency List

An adjacenncy list is a collection of linked lists that show the Edges for every node.

## Weighted Graphs

In a weighted graph, the edges have a value associated with them, which can be represented on the adjecency matrix with the value instead of a 1, or in an adjacency list by including the value at each node in each linked list.

## Traversals

### Breadth first

Start at some root node, and traverse like you would through a tree using a Queue. You must also keep track of which nodes you've hit to avoid infinite loops in a cyclic graph.

This wont traverse seperate islands, or nodes that are not connected in some way to the original root node.

### Depth first

This time, we'll use a Stack rather than a Queue.

push some root node into the stack,
then while the stack is not empty, peek at the top node, and if it has unvisited children push them onto the stack.
If is doesn't have any unvisited children, pop the top off that stack.
repeat till the stack is empty.

[<--- Back](../README.md)

# stacks and queues

Stacks are very similar to linked lists that we've been learning about.

As you add Node to a stack they should point to the pre-existing top of the stack if one exists. You can then pop the new top, and the old one would take its place as the top.

You can think of a stack like any stack of objects in the real world I like to compare it to a stack of pancakes. One pancake gets set down, then another one on top, then another and so on. Then you can remove the topmost pancake, to reveal the one beneath it.

```asciiart
TOP  C
     ^
     B
     ^
     A
```

Stacks are a First In Last Out data structure.

Queues are also similar, however they are a First In First Out Data structure. More like cars at a stop light, as a new car rolls up, it has to stop behind all the other cars ahead of it. When the light turns green, the first car to get going is the car in the front of the queue.

In a queue, each node holds a pointer to the node behind it, and the queue itself holds a pointer to both the front and also the rear.

```asciiart
 REAR     FRONT
  C <- B <- A
```

[<-- Back](../README.md)

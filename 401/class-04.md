# Classes and Objects

Objects are collections of data and methods to interact with that data and other objects.

Classes are the definition or the blueprints of objects.

Accessing variables in an object is easy:

`some_object.the_variable`

Calling a method:

`some_object.a_method()`

Instrances of objects have their own values associated with their variables.

## recursion

Recursive functions divide a larger problem into smaller chunks, and then call themselves to attack those smaller chunks, which call themselves to attack even smaller chunks, etc

Each recursive call addes its own execution frame on the stack.

If you want persistent data through recursion you have to either pass that data through the recursive calls OR maintain that data at a global scope.

Some data structures themselves can be recursive in nature, like a file structure tree.

## Caching

You can use a `@lru_cache` decorator in python to allow recursive functions to cache their results, so that we dont have to run the same logic over and over if a previous case handled it. This is demonstrated in a fibonacci series: fib(4) contains fib(3), and fib(2)... and  fib(3) contains fib(2), so if we could cache fibi(2) and only need to run that execution once, then lookup any subsequent calls to fib(2), then we'll have improved performance (at scale)

[<-- Back](../README.md)

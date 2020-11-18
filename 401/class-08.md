# List Comprehensions and Decorators

## List Comprehensions

List comprhension are a way of building a list based on some criteria.

Implementation:

```python
some_list = [ expression for item in list if condition ]
```

some examples:

```python
# build a list from 0 - 99
result = [ i for i in range(100) ]

# cubes of values 0-9
result = [ x**2 for x in range(10) ]

# chars in a string, exluding spaces
result = [ c for c in "blah blah blah" if c.isalpha() ]

# multiply the coefficients of two polynomials
result = [ x + y for x in [1, 2] for y in [3, 4]]
```

## Decorators

First, in Python functions are *first-class objects* which means that they can be passed around and used as arguments, and even returned from other functions.

Now decorators are just a way to wrap a function, and modify behavior.

```python
def do_something(some_func):
    def my_decorator():
        some_func()
    return my_decorator

@my_decorator
def do_something(some_func):
    some_func()
```

Decorators can take arguments using *args and **kwargs.

You can stack multiple decorators on top of eachother, in which case ordering matters.

You can even use a class as a decorator to maintain state.

[<-- Back](../README.md)

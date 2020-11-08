# Python Names (variables)

You can use [Python Tutor](pythontutor.com) to visualize your code, and how assignments are being made as you step through it.

## Names

Names (variables) are reassigned independently:

```python
x = 10
y = x
x = 13
# y still refers to 10, even though x has been reassigned to 13
```

In Python, assignment never copies data, i.e.:

```python
set1 = [1,2,3]
set2 = set1
set1.append(4)l
print(set2) #prints [1,2,3,4]
```

## Immutable vs Mutable

In python, ints, floats, strings and tuples are immutable.

This can be a bit confusing because when we do some operations like:

```python
x = 1
x = x + 1
```

x is set to 1, then re-set to 2

Other datatypes are mutable, like list, we saw a good example of that above.

## References

Lots of things are references in Python

- object attributes
- list elements
- dictionary values and keys
- anything on the left side of an assignment operation

## Assignments

There are a lot of ways to assign in python.

```python
X = blah
for X in blah ...
class X(...):
def X(...):
# etc
```

When nothing is assigned to a value anymore, garbage collection kicks in allows that memory for the value to be reallocated.

[<-- Back](../README.md)

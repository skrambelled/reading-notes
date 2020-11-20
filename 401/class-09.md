# Dunder methods

Sometimes reffered to as *magic* or *special* methods, dunder methods are predefined methods in Python indicated by their double underscore or **dunder** naming convention.

We've already been exposed to `__init__`, `__repr__` and `__str__`

Dunder methods allow classes to emulate builtins


dunder | what it does
------ | -------
`__init__` | object initialization
`__repr__` | representation of an object or class
`__str__` | `str(ob)`
`__len__` | `len(ob)`
`__getitem__` | `ob[start:stop]`
`__reversed__` | `ob[::-1]` \| `reversed(ob)`
`__name__` | name of the class
`__eq__` | `==`
`__lt__` | `<`
`__gt__` | `>`
`__add__` | `+`
`__call__` | `ob()`

There are tons more, just look them up!

[<-- Back](../README.md)

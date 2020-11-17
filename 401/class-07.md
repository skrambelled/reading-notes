# Python Scope

## LEGB

* local (or function) scope
* enclosing (or nonlocal) scope
* global (or module) scope
* built-in scope

The term `name` in python refers to the identifier of variables, constants, functions, objects, classes in Python

Python will look through those scopes in LEGB order for a given name and return the first occurrance or an error of it does not exist.

Avoid using global scope. It creates code that is dependant on a specific application rather than allowing code to be re-useable.

You can import built-ins specifically, so that they can take precedence over global scope of the same name.

You can declare a name as `global` within a local scope so that a new local name is not created, but instead you refer to the globally scoped one. If you declare a variable as global in a local scope that does not exist globally, it will be scoped to the global namespace, known as lazy globals. **BE VERY WARY OF DOING THIS!!**

similarly you can declare a name as `nonlocal` within a inner function to allow you to interface with them. You cannot make lazy nonlocals.

## Namespaces

In Python scopes are implemented as dictionaries, where names are keys, and their objects are the values of the key-value pair system.

`some_module.__dict__` will give you access to this dictionary for any given module.

[<-- Back](../README.md)

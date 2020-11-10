# Recursion, testing and modules

## Recursion

Recursion is when a function calls itself, either directly or indirecly. In recuresion, the base case it the problem expressed in its smallest form, and which can be called recursively, for example:

Summing all the numbers in a series of consectutive integers starting at 1, 1 is the base case.

n | equation | sum
- | -------- | ---
1 | n | 1
2 | 1 + n | 2
3 | 1 + (1 + n) | 6
4 | 1 + (1 + (1 + n)) | 10
5 | 1+(1+(1+(1+n))) | 15

When no base case is defined, or is never reached, we'll run the recursion infinitely.

Recursion requires more space because each function gets allocated on top of the previous one, and must be resolved before we return down. All recursive code can be coded iteratively, but recursion can be simpler to code. It is preferable to code when the problem it solves is inheritanly recursive.

## Testing

*Test Driven Development* means writing the tests for code before even writing the code.

Tests should live in their own dir structure outside of the actual production code. Tests should be simple. Function and variable names should be specific, the code itself is its own documentation. Test files shold be named after the module they are testing, for example:

```
somedir/
  a_module.py
tests/
  test_a_module.py
```

The coding of complex ideas can be broken down into babysteps, and TDD can be a useful tool in that process.

## Modular programming

Break a complex programs into smaller modules, so that problem are easier to code, reused or worked on.

Modules can be written in python, in C and loaded into python runtime, or built into the interpretter.

[<-- Back](../README.md)

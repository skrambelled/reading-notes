# The call stack

JavaScript is ran in a single-threaded environment, which means only one operation can happen at a time, before the next one can.

When you call a function, it goes on the 'stack', like a stack of pancakes. If that function calls another function inside of it, then that second function is like another pancake being tossed on top of the previous one. The most recent funcion is always on top, and must be resolved before we can go deeper down the stack. This is a first-in-last-out approach.

A stack overflow can happen if a function calls itself recursively without any exit point, meaning you get an infinite stack. (environments can define their stack to something other than infinite, so that they can throw an error at some point).

## Errors

### Reference error

When you try to use a variable that is not declared, for example, if it is not withing the same scope.

### Syntax error

When the parser runs into some syntax that it cannot resolve, like trailing commas or missing semi-colons. Browsers often will try to resolve this bad syntax as best they can, but really you should just be accurate in your code.

### Range error

Using something outside of an expect range, like trying to reference a negative index on an array.

### Type error

Trying some operation on a value of the incorrect type. like `NaN + 1`;

## Error handling

We can use try-catch blocks to handle errors, and give us accurate information about an error.

```js
try {
  some_code_that_might_produce_an_error();
}
catch(error) {
  console.error('we had an error with some_code...()', error);
}
```

[<-- Back](../README.md)
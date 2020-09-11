# Debugging JS

## Order of execution

- Javascript has a global context, where functions are declared and executed at a global level. Variables are at global scope at this level.
- Function context where code is being run in a function, every function has its own function context. Variables are at Function level scope in this context.
- Eval context, like a function inside a function.

JS executes code in a stack. like a stack of pancakes. each pancake is a function, when you call a function you put a pancake on the plate. If that function calls a new function you put a new pancake on top of the existing pancake. When that function is done executing, you eat that top pancankem then you can eat the first pancake. Huzzah!

WHen a new execution context is created, there are two phases:

1. Prepare
   - A new scope is created
   - variables functions and arguments are created
   - the `this` keyword gets a value determined

2. Execute
   - Assign value to variables
   - Reference functions
   - execute statements

## Scope

JS has lexical scope, meaning variables defined in parent functions can be access by children function, but not the other way around, but reaching upwards to parents or grandparents can be expensive, so usually define pass those as parameters down to children if you need access, and return them back out to parents if you need to traverse back up.

## Errors and Exceptions

WHen JS encounters an error, it will throw an error exception, and stop running the execution. You can `handle` an error to keep running at the parent scope of the error-handling code.

### Error objects

When an error occurs, and Error object is created. There are 7 built in objects:

object | description
------ | -----------
Error  | base error object
SyntaxError | JS syntax is not correct
ReferenceError | tried to access a variable that does not exist at this scope
TypeError | data type that cannot be coerced for whatever operation you are doing
RangeError | number not in range
URIError | bad URI encode or decode
EvalError| eval() func error

### Debugging

- Use dev tools in browsers to navigate the code and the DOM to find errors.
- Try to describe the logic out loud, as you go through the error area.
- Call functions in the console to see their behavior.
- Look at objects and their methods in the dev tools.
- Keeps notes when debugging longer blocks of logic about what you have and have not tested so you can keep track.
- Try another browser to gain insight.
- `console.log()` some error breadcrumbs.
- `console.info()`, `console.warn()`, and `console.error()` can give your console output some more visual context to assist debugging.
- `console.group()` and a corresponding `console.groupEnd()` can can make collapsable console entries.
- `console.table()` allows for tabular data in your console output.
- `console.assert()` to output to console conditionally.
- Use breakpoints to pause execution, so you can inspect variables.
  - Chrome -> Inspect -> Sources
  - Firefox -> Inspect -> Debugger
  - `debugger;` keyword in JS will also be a breakpoint
  - Stepping
    - pause
    - step through
    - step into
    - step out
  - Conditional breakpoints can be done in JS using the `debugger` keyword inside of logic, or through mouseclicking through dev tools

### Error handling

```js
try {
  thisCode();
} catch (exception) {
  run_this_if_exception();
} finally {
  always_run_this_code();
}
```

You can `throw` an error object when you know something is wrong, rather than waiting for an error to occur later on down the road.

[<-- Back](../README.md)

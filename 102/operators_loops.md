# Operators

## Comparative and logical operators
```js
`>` /* greater */
`<` /* less than */
`>=` /* gt or equals */
`<=` /* lt or equals */
`==` /* equals */
`===` /* equals and also same type */
`!=` /* not equals */
`!===` /* not equals or not the same type */
`&&` /* and */
`||` /* or */
`!` /* not */
`=` /* variable assignment */

```
## String operators
```js
`+` /* concatenate two strings */
```

## Arithmetic operators

```js
`+` /* addition */
`-` /* subtraction */
`*` /* multiplication */
`/` /* division */
`%` /* modulus */
`++` /* increment */
`--` /* decrement */
```

## Bitwise operators

```js
`|` /* or */
`&` /* and */
`~` /* not */
`<<` /* bitshift left */
`>>` /* bitshift right */
```

# Loops

Loops are used to run code multiple times while a condition evaluates as `true`.

## `for()`
Used when you need to run code a specific number of times.
```js
// countdown from 10 to 0
for( var countdown = 10; countdown >= 0; countdown--) {
  console.log(i);
}
```

## `while`
Used when you do not know how many times you need to call the loop.
```js
// countdown from some priorly set countdown value
while(countdown >= 0) {
  console.log(countdown);
  countdown--;
}
```

## `do-while`
Similar to while, run code for an unknown number of times, but run the code at once initially, even if the conditiion is false.
```js
// countdown from some priorly set value, even if we start at 0
do { 
  console.log(countdown);
  countdown--;
} while(countdown >= 0)
```

[<= Back](README.md) 
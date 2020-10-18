# Refactoring

Good code finds a balance between speed and maintainability.

Often writing code quickly will produce illegible code, even if it works.
Or if the focus is too heavily weighted towards maintainability then product will be too slow.

## Examples

### Return early

```js
// Instead of:
if(something) {
  do_thing();
}


// return early:
if(!something)
  return;

do_thing();
```

This may seem small now, but as your codebase grows a practice of returning early will keep your code neat.

### Cache variables

```js
//Instead of:
for(let i=0; i<thing.length; i++)
  for(let j=0; j<thing[i].length; j++)
    for(let k=0; k<thing[i][j].length; k++)
      action(thing[i][j][k]);

// cache variables to be more legible
for(let i=0; i<thing.length; i++;) {
  let other = thing[i]; // cached
  for(let j=0; j<other.length; j++) {
    let more = other[j];
    for(let k=0; k<more.length; k++) {
      action(more[k]);
    }
  }
}

```

[<-- Back](../README.md)
# Lists, Boxes, Loops

## Lists

An unordered list will use bullets to list the items:

```html
<ul> <!-- unordered list -->
  <li>list item 1</li>
  <li>list item 2</li>
</ul>
```

An ordered list will enumerate the items:

```html
<ol> <!-- ordered list -->
  <li>list item 1</li>
  <li>list item 2</li>
</ol>
```

Definition lists use definition terms and definitions of those terms:

```html
<dl> <!-- definition list -->
  <dt>Some term</dt>
  <dd>the definition of the term</dd>
</dl>
```

Lists may be nested, so that sub-lists will be indented further than the parent.

## Boxes

In HTML, nearly evcerything is separated into logical containers or boxes.
Boxes are by default, only as large as the content that they contain, but designers can manage their size manually, and these rules are typically applied through CSS using properties such as:

- `height`
- `width`
- `max-width`
- `min-width`
- `min-height`
- `max-height`
- many more!

Every box has three properties surrounding the internal content:

- `margin`
- `border`
- `padding`

Boxes may also appear inline or at a block level. Certtain HTML elements default to inline or block level, but that property can typically be overridden.

There are a variety of properties that can be applied through CSS to control each of the properties in specific or even dynamic ways.

## Javascript Decisions and Loops

### Conditional statemants

```js
if(expression) {
  do_this_if_true();
} else {
  do_this_if_false();
}
```

```js
switch(expression) {
  case some_condition:
    do_this_thing();
    break; // unless you want to fall through to the next case

  case some_other_condition:
    do_this_other_thing();
    break;

  default: // we did not match an conditions
    do_this_thing_that_no_other_conditions_met();
}
```

### Loops

```js
// run for a specified number of times
for(var i = 0; i<10; i++>) {
  do_this_thing_10_times();
}
```

```js
// keep running while expression is true
while(expression) {
  repeat_this_thing();
}
```

```js
// keep running while expression is true, but run once even if its not
do {
  do_this_thing_once_at_least();
} while (expression);
```

### Truthy and Falsey

All values have some truthy or falsiness to them. For example:

type or expression | value | boolean truthy/falsey
---- | ----- | -------------
number | `2` | `true`
string | `" "` | `true`
string | `"false"` | `true`
string | `""` | `false`
boolean | `false` | `false`
(expression) | `80 === "80"` | `false`
(expression) | `80 == "80"` | `true`
(expression) | `false || true` | `true`

[<-- Back](../README.md)
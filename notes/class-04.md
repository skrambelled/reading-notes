# Functions, Pair Programming, Layout

## JavaScript Functions

Functions in JS are bits of code that perform a specific task.
Methods are functions that are part of an object.

A function is especially useful when you might need to call it over and over again.

A method is useful for getting information about or manipulating variables of an object.

An example of a js function that returns the absolute value of a number,
in this case `abs` is the name of the function, `i` is the parameter, and we `return -i` or `return i` depending on the internal code of the `abs()` function.

```js
function abs(i) {
  if(i<0)
    return -i
  return i;
}
```

You can return an array out of a function if you needed more than a single value.

You can also return objects, or any other data type.

Anonymous functions (functions that are not named) are "Immediately Invoked Function Expressions" or "IFFE".

```js
var density = (function() {
  var mass = 100;
  var volume = 25;

  return mass/volume;
} () );
```

Variables declared inside of a function are only accessible within the function, this is called 'local scope'.

Variables declared outside of a function have 'global scope'. They will take up memory, so use sparingly.

---

## Pair programming

Pair programming is a common practice for agile environment. This is when two people share a workstation and program together as a pair.

It allows for real-time error and typo checking. Big picture thinking. Keeping track of the code using the simple "two heads are better than one" approach to problem solving.

There are two roles in pair programming:

- Driver (hands on the keyboard, doing the actual coding, file system navigation, version control)
- Navigator (verbally assisting, keeping track of the big picture, thinking about what comes next, typo checking, etc)

Pair programming is also very useful in learning a new language because it utilized multiple and critical learning skills:

- Listening
- Speaking
- Reading
- Writing

Additionally, in a learning environment especially pair programming help:

1. Efficiency
   - even though it may take longer inititally, debugging is faster and the initital code is of higher quality because two people had their eyes and brains on it.
2. Engaged Collaboration
   - When you are working actively with someone, you are less prone to distraction.
3. Learning
   - You have an instant resource for helping figure out how to solve problems.
4. Social Skills
   - Both parties will improve their communication skills.
5. Job interview readiness
   - Interviews commonly use pair programming as part of their process to see how you might fit into their team.
6. Work envirnment readiness
   - Once in a work environment, pair programming is often utilized for training new people. Having already practiced the general format of pair progamming you will be prepared for this.

---

## Links

Links are a core concept of the web, and they tie the web together. (Hence the word 'web')

There are a variety of links.
- email apps
- from one part of a page to another in the same page
- between web pages
- to external web sites
- new browser windows

An example of a link to google's home page:

```html
<a href="http://google.com">google</a>
```

An exampple of an email link:

```html
<a href="mailto:skrambelled@gmail.com">Email Me</a>
```

---

## Layout

Layout of a site is handled by the relationship of HTML and CSS

There are two levels of elements:

- Block
- Inline

Every block-level element will appear on a new line whereas inline elements will not.

CSS allows for 3 position schemes

Normal flow, Relative positioning, and Absolute positioning.

There is also a z-index to control the 'depth' of elements on the page.

This whole Layout sctructure will take practice! practice! practice! to learn.

[<-- Back](../README.md)
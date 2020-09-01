# Introduction to HTML, CSS and JavaScript

## HTML (Hypertext Markup Language)

HTML is the language responsible for organizing the content of a web page.

- Content is organized by HTML elements, `<h1>` (main heading) or `<p>` (paragraph).
- Elements may have attributes, like class or language.
- Any HTML page should have at least:
```html
<html>
  <head>
    <title>Some title</title>
  </head>
  <body>
    <h1>Main heading</h1>
  </body>
</html>
```
- There are block level elements, which will always display on a new line, and also inline elements which will be displayed inline. You can usually modify the default of any given tag.
- HTML5 introduced many layout elements, such as:
  - `<header>` and `<footer>`
  - `<article>`
  - `<nav>`
  - `<aside>`
- There are many many elements, so look them up and try them out!

## CSS (Cascading Style Sheets)

CSS is the language that manipulates the style and layout of a web page.

- CSS is made of of selectors and attributes:

```css
p {
  color: blue;
}
```

`p` is a selctor for all the `<p>` elements.
`color` is the attribute we are modifying.
`blue` is the value we are assigning to `color`.



## JavaScript

While HTML is the content layer and CSS is the presentation layer of a web page, JavaScript is the behaviour layer.

JavaScript allows you to dynamically interact with the user in a page.

JS is an object oriented language.

JS runs where it is found in the HTML.

```js
/* comment in JavaScript */
```

## How to use JavaScript

You will need to insert a `<script>` tag into your html, and then point that to your .js file using the src attribute.

##  Variables

JS allows you to declare a variable and also assign it a value inline:
```js
var text = "This is a test!";
```
### Types
Javascript utilizes a few core data types for its variables:
- null
- boolean
- number
- string
- array
- function
- and of course, objects

All variables in JS are dynamically typed however you can use the `'using strict'` at the top of a .js file to force mor
e tight control over data type comparisons and uses.

### Naming
* Variables must begin with a-z, $, or _ characters, and must **NOT** start with a number.
* Can contain a number later, but **NOT** a `.` or `-`
* Can **NOT** be a *keyword* or *reserved* name.
* Case sensitive.
* Should be concise, but also descriptive.
* shouldUseCamelCase but start with lowercase, or use underscore_naming_style


[<-- Back](../README.md)
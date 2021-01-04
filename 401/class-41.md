# React

## JSX

> `const element = <h1>Hello, world!</h1>;`

This is neither a string and also not HTML, but is instead JSX or JavaScript XML, and called a React Element.

You can put any valid JS expresions inside of `{}` curly braces of JSX.

You can split JSX over multiple lines, but when doinng so, wrap the entire JSX expression it paranthesis, so that you do not get automatic semi-colon instertions from a browser trying to be too smart.

```js
// You can use "quotes" to specifiy attributes
const element = <div class="something"></div>

// you curlies to insert js expressions
const element = <img src={myimage.png}></img>

// but don't use "{}" qoutes aorund curlies
```

The React DOM escapes embedded value in JSX, so you are able to embed user imput directly into your JSX without fear of malicious code, which prevents Cross Site Scripting attacks.

## React rendering

JSX elements are objects. But to render them onto a page, we need to pass them to the ReactDOM's `render()` method.

React updates only the necesary elements rather than the whole page.

## Functions and Class Components

React components must start with a capital letter, otherwise they will be treated as a DOM tag.

Components can be comprised of multiple smaller components.

Components have properties, or props, and the convention is to name those props from the perspective of the component.

All React components must act as pure functions for their props, meaning they cannot change state of their own props. To change state, we'll use a different approach, using classes.

## Lifecycle

Components in React should be cleaned up so they don't use up resources when unneeded. You `mount` some component, but then `unmount` it when you clean up after a component.

## Events

Events in React are similar to events in the normal DOM, but they use camelCase, instead of lowercase. Additionally, When using JSX, you pass a function instead of a string.

Instead of calling `addEventListener()` like you would in JS, you can define events in your render method in a component.

[<-- Back](../README.md)

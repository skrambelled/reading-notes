# Problem Domain, Objects, DOM

## Problem Domain

The Problem Domain is often the hardest part of programming, its easy to make assumptions about what you knwo and just hit the ground running, only to later realize that you've not understood the issue you are trying to solve or the product you are making well enough, and then you have to start over agian.

When learning to program, removing the problem domain by making it explicit or simple can put you directly in contact with the programming concepts

When you need to understand the Problem Domain, you can chunk it into smaller pieces and learn those domains first before expanding outwards.

## Objects

In an object variables are called properties, and functions are called methods.

An example of a pizza object:

```js
var pizza {
  slices: 8; // this pizza starts with 8 slices
  
  // a method to remove 1 slice
  removeSlice: function() {
    if(this.slices)
      this.slices--;
  }

  // a method to query how many slices this pizza has
  querySlices: function() {
    return this.slices;
  }
}
```

```js
var slices = pizza.slice()
```

## DOM

The Document Object Model or DOM refers to the object tree that defines the space of a web page loaded into memory from a browser and how JavaSCript can reference object within that tree.

A DOM tree starts with the document object at the top, and then elements listed as nodes nested beneath. Each node may have an attribute node and a text noded associated with it.

There are lots of ways to access the elements, like:

- `getElementById()`
- `getElementByClassName()`
- `querySelector()`
- `querySelectorAll()`

## nodelist

When accessing elements, you may get a node or a node list when mutiple nodes are accessed.

- `nodeArray.item(0)` will access the node in the nodelist at index of 0
- `nodeArray[0]` will do the same, bvut faster
- `nodeArray.length` return the size of the nodeArray

## Traversing the DOM

- `parentNode`
- `previousSibling`
- `nextSibling`
- `firstChild`
- `lastChild`

## modifying nodes

- `nodeValue` only on a text node
- `innerText` access the text content, ignoring any CSS rules
- `innerHTML` careful of security issues, as you can expose yourself to injection here, but innerHTML can be used to modify entire DOM sub-trees

## adding nodes

- `createElement()`
- `createTextNode()`
- `appendChild()`

## XSS or cross site scripting

Never trust non-validated data, like user generated content. This can lead to vulnerabilities.

Never allow user input to allow javascript, escape chars, or markup.

You can accomplish this by validating or excluding input, but you have to do it at the sever level to defend against users that have their JavaScript turned off.

## Chroms

You can inspect a page in chrome to look at the DOM.

[<-- Back](../README.md)
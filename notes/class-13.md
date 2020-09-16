# Local storage

Historically, native applications have had an advantage because they can store data locally in a number of ways.

Web applications have used cookies for storage, which can store a small amount of information, but are innefficient because you need to transfer them frequently.

There have been advances over the years with a variety of technoologies that allows web apps to store data locally on the clientside, with varying degrees of success.

One of HTML5's goals was to create a uniform API to address clientside storage issues in a consistent user experience.

## HTML5 storage

`window.localstorage` will allow JS access to storage on the browser.

Storage is in the form of key-value paits, where the key is a string, and the value can be of any type. However the value is typically stored as a string so you will need to parse it back into the correct data format.

You can use bracket notation or the `setItem()` method to store data:

```js
window.localStorage.setItem("key", value);

window.localStorage["key"] = value;
```

Similarly, to retrieve data:

```js

var value = window.localStorage.getItem("key");

value = window.localStorage["key"];

```

## Limitations

- 5 MB per origin
- "QUOTA_EXCEEDED_ERR" is the error when you exceeed that MB limit
- You cannot request more space
(I question this, as the book is a few years old, and I expect this may have changed since then)

- There is some support for aa variety of actual DB storage, such as SQLite.

[<-- Back](../README.md)

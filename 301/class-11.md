# Embedded JavaScript and Google Books API

## EJS

EJS is a way to insert JavaScript directly into html as a template.

`<% embedded_js_code_here %>`

### tags

* `<% %>` - no output
* `<%= %>` - outputs value
* `<%- %>` - outputs value (not HTML escaped)
* `<%# %>` - comment
* `<%%` - literal <%
* `<% %>` - no output
* `<%_ %>` - strip preceding whitespace
* `<% _%>` - trim trailing whitespace
* `<% -%>` - trim trailing newline

Ejs seems to be a way to get some simple javascript embedded into your html, good for some quick lifting, but not for more cmplex stuff.

### [example app](https://github.com/scotch-io/node-ejs)

Read through this small Node app which demonstrates doing some layout with EJS. It breaks some portions of the page into smaller parts, and then injects them in specific spots in the html. I am imagining how this might be useful in conjunction with CSS.

## Google Books API

* __Volume__: this is all the data about any particular book or magazine
* __Bookshelf__: a collection of volumes, can be manually or automatically stocked, or a mix of the two
* __Review__: user generates star rating and/or text, 1 per volume max
* __reading position__: The last read position of a given user
* __resources__ are consider volumes and bookshelves

### API operations

* __list__ - get resources (volumes or bookshelves)
* __insert__ - insert bookshelves, reading positions
* __get__ - get resources, and reading positions
* __update__ - update bookshelves, reading postions
* __delete__ - remove bookshelves, reading postions

[Authentication](https://developers.google.com/books/docs/v1/using#auth) is required for some of the these actions.

All data is in json format when using the API.

[<-- Back](../README.md)

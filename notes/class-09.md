# Forms and Events

## Forms

Forms are a way for the user to input text into a page.

- text
- radio buttons
- dropdowns
- buttons

### Form controls

Every `<form>` will have an `action` attribute, which refers to the page that receives the forms input.

Every form usually has a `method` and `id` attribute as well.
The method attribute can be `"get"` or `"post"`.

- `"get"` will append the form values to the URL
- `"post"` will use http to move information

#### Input

`<input>` can be assigned attributes to determine how the form will work.

- `type`
  - `"text"`
  - `"password"` (will mask the characters on the screen, but still requires an SSL to send the data securely)
  - `"radio"` single selection checkbox
  - `"checkbox"` multiple selection checkbox
  - `"file"` allow users to selct a file on their system
  - `"submit"` a button to submit the form to the server
  - `"image"` a button with image to submit the form
- `name`
- `maxlength`
- `size` (deprecated, use CSS to set the size)

`<textarea>` can be used for multi-line inputs.

`<select>` dropdown menu

- `<option>` to make items for the menu

### Form validation

HTML 5 can vlidate form input to some degree, but JS can also do this job in a more robust way.

Some HTML form vaildation options include:

- required
- date
- email

## Events

Events allow your JS to interact with the user through the browser when certain actions take place to create an interacite page.

Thers is a huge list of events ranging from loading the page to keyboard or mouse events. Just look up a big table of these events and try to use each one.

When events occur, it is called firing or raising.
An event is fired or raised in other words.

There are 3 steps for an event:

1. an element or node is associated with an event
2. a event type is associated
3. some code is assosiated

For example, on a particular `<p>` node, you might have a `mouseover` event, which calls some JS to change the contents.

There are 3 ways to bind an event to a node or element.

1. HTML event attributes (deprecated DO NOT DO THIS)
   - `<element onclick="someCode()">`
2. DOM event handlers (only a single event can be bound)
   - `element.onclick = someCode;`
3. DOM level 2 events OR listeners (preferred way, multiple scripts can be nound)
   - `element.addEventListener('onclick', someCOde, false);`
     - false -> bubbling
     - true -> capturing

### Event Flow

Flow can be inwards, which is called bubbling.
Or it can be outwards, which is called capturing.

Event Delegation allows you to associate events in a parent-child relationship rather than having an event for each node you want to make an event for, which would be expensive.

[<-- Back](../README.md)

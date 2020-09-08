# Tables and Constructors

## Tables

Tables are simply information in a grid format consisting of rows, and within each row, table data (or you might call them cells).

### Creating a table using 4 key elements

1. `<table>` container for the table
2. `<tr>` table row
3. `<td>` table data, or cells within each row
4. `<th>` table heading, to label rows or cols

Attributes

- `colpan=X` spans X table data cols when applied to a `<td>` element
- `rowspan=X` spans X table rows when applied to a `<tr>` or `<th>` element

Extra elements for better styling and screenreader support:

- `<thead>`
- `<tbody>`
- `<tfoot>`


### Represent complex data in a table

## Constructors

Instantiating a function expression:

```js
var Car = function(year, make, model, color) {
  this.year = year;
  this.make = maker;
  this.model = model;
  this.color = color;
}

var myCar = new Car(1994, "toyota", "Camry", "red");
```

Prototyping

```js
// using the Car fucntion expression from above
Car.prototpye().randColor() {
  ['red','green','white'][Math.floor(Math.random()*3)];
}

var yourCar = new Car(2001, "Honda", "Civic", randColor());
```

`this` is a keyword that represents the current object.

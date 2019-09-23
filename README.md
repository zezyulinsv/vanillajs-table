### vanillajs-table

> version 0.1.0

Library to create HTML-tables by vanilla JavaScript.

#### Installation:

-   include `vanillajs-table.js` file:

```html
<script type="text/javascript" src="src/vanillajs-table.js"></script>
```

#### Basic usage

Use minimalism code:

```javascript
new Table({
    element: document.getElementById("container"),
    data: [1,2,3,4,5]
}).view();
```

Or use detailed code:

```javascript
var table = new Table();

// Set table parameters.
table.element = document.getElementById("container");
table.data = [1,2,3,4,5]

// Visualizing the table.
table.view();
```

#### Options

Available options listed below.

```javascript
new Table({
    headers: [                  // {Array} header parameters
        {name: "Title"},        // - {Object} first column parameters
        {name: "Artist"},       // - {Object} second column parameters
        ...
    ],
    element: Element,           // {Element} DOM Element to insert the table
    data: [],                   // {Array|Object} data
    height: 400,                // {Number|String} maximum table height
    undefined_headers: true,    // {Boolean} show undefined headers
    empty: "----"               // {String} instead of an undefined value
});
```

### Converting an multiple array to a table.

#### HTML code

```html
<!DOCTYPE html>
<html>
    <head>
        <script type="text/javascript" src="src/vanillajs-table.js"></script>
    </head>

    <body>
        <div id="table"></div>
    </body>
</html>
```

#### JavaScript code

```javascript
var eats = [
    ['Apple', 'Banana', 'Orange', 'Blackberry'],
    ['Cabbage', 'Turnip', 'Radish', 'Carrot']
];

var options = {
    element: document.getElementById("table"),
    data: eats
};

var table = new Table(options);

table.view();
```

#### Result

| 0       | 1      | 2      | 3          |
| ------- | ------ | ------ | ---------- |
| Apple   | Banana | Orange | Blackberry |
| Cabbage | Turnip | Radish | Carrot     |

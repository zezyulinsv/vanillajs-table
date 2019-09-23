### Converting an array to a table.

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
var fruits = ['Apple', 'Banana', 'Orange', 'Blackberry'];

var options = {
    element: document.getElementById("table"),
    data: fruits
};

var table = new Table(options);

table.view();
```

#### Result

| (values)   |
| ---------- |
| Apple      |
| Banana     |
| Orange     |
| Blackberry |

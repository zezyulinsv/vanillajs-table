### Converting an object to a table.

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
var song = {
    title: "Le Roi Est Mort, Vive Le Roi!",
    year: 1996,
    project: "Enigma"
};

var options = {
    element: document.getElementById("table"),
    data: song
};

var table = new Table(options);

table.view();
```

#### Result

| title                          | year | project |
| ------------------------------ | ---- | ------- |
| Le Roi Est Mort, Vive Le Roi!" | 1996 | Enigma  |

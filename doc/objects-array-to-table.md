### Converting an objects array to a table.

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
var discography = [
    {
        album: "MCMXC a.D.",
        year: 1990
    }, {
        album: "The Cross of Changes",
        year: 1993
    }
];

var options = {
    element: document.getElementById("table"),
    data: discography
};

var table = new Table(options);

table.view();
```

#### Result

| album                | year |
| -------------------- | ---- |
| MCMXC a.D.           | 1990 |
| The Cross of Changes | 1993 |

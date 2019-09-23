### Pre-installed headers.

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
var artists = [
    ["Andy Warhol", "1928-1987"],
    ["Jan van Eyck", "1390-1441"],
    ["El Greco", "1541-1614"]
];

var headers = [
    {name: "Artist"},
    {name: "Lifetime"}
];

var options = {
    element: document.getElementById("table"),
    headers: headers,
    data: artists
};

var table = new Table(options);

table.view();
```

#### Result

| Artist       | Lifetime  |
| ------------ | --------- |
| Andy Warhol  | 1928-1987 |
| Jan van Eyck | 1390-1441 |
| El Greco     | 1541-1614 |

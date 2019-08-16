# defineFilter

```javascript
Sqrl.defineFilter("filtername", function (str) {
        // Do something with string
        return str
})
```

## Examples

```javascript
Sqrl.defineFilter("reverse", function (str) {
    var out = ''
    for (var i = str.length - 1; i >= 0; i--) {
        out += String(str).charAt(i)
    }
    return out || str
})
```


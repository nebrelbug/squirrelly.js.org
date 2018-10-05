---
description: The syntax of Sqrl.defineFilter
---

# defineFilter

```text
Sqrl.defineFilter("filtername", function (str) {
        str = str.replace("filtervalue", "")
        return str
})
```

## Examples

```text
Sqrl.defineFilter("reverse", function (str) {
var out = ''
for (var i = str.length - 1; i >= 0; i--) {
    out += String(str).charAt(i)
}
return out || str
})
```


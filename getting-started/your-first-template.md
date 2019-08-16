# Your First Template

## Browser Demo

{% embed url="https://runkit.com/nebrelbug/squirrellyjs-basic-example/4.0.1" caption="" %}

## 1. Install Squirrelly

Follow the [installation instructions](installation.md), then require or import Squirrelly. In this example, we'll require Squirrelly as the variable `Sqrl`.

```javascript
var Sqrl = require("squirrelly")
//Or you could: import * as Sqrl from "squirrelly"
//Or, if you're in the browser, Sqrl is already global
```

## 2. Create a Template

```javascript
var myTemplate = `
This is a template
My favorite template engine is: {{fav}}
My favorite kind of cake is: {{cake}}
`
```

{% hint style="info" %}
In this example, we're using JavaScript template literals. **You don't have to use template literals with Squirrelly**. It just makes it easier to write templates, since you don't have to escape newlines. In real life, most templates are their own files.
{% endhint %}

## 3. Render your Template!

```javascript
var templateResult = Sqrl.Render(myTemplate, {
    fav: "Squirrelly", cake: "Chocolate"
})
console.log(templateResult)
//This is a template
//My favorite template engine is: Squirrelly
//My favorite kind of cake is: Chocolate
```

Try rendering it with other data: it still works!


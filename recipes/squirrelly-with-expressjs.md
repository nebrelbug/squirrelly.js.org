# Squirrelly with ExpressJS

{% hint style="info" %}
Since Squirrelly exports the `__express` helper, it works out-of-the-box with Express.
{% endhint %}

{% hint style="info" %}
Though Squirrelly handles caching, it isn't very sophisticated and the cache only lives for the life of the program \(it's stored in a variable\). You may want to implement your own caching solution.
{% endhint %}

{% code-tabs %}
{% code-tabs-item title="index.js" %}
```text
let express = require('express');
let path = require('path');
let app = express();

app.set('view engine', 'squirrelly')

app.get('/', function (req, res) {
    res.render('index', {
        name: 'Title',
        fav: 'Squirrelly'
    })
})

let server = app.listen(4000, function () { // This starts the server
    console.log("listening to request on port 4000");
});

```
{% endcode-tabs-item %}
{% endcode-tabs %}

{% code-tabs %}
{% code-tabs-item title="views/index.squirrelly" %}
```text
<!DOCTYPE html>
<html>
<head>
    <title>{{name}}</title>
</head>
<body>
<p>My favorite template engine is {{fav}}</p>
</body>
</html>
```
{% endcode-tabs-item %}
{% endcode-tabs %}




---
description: The syntax of Sqrl.Compile
---

# Compile

{% hint style="info" %}
Many template engines offer you the option to **Compile** \(which just renders your template\) or **Precompile** \(which turns your template into a function ahead of time\). Squirrelly precompiles **automatically,** but is still faster than other engines.
{% endhint %}

## Syntax

```text
var myTemplate = "Hi, my name is {{name}}"
var compiled = Sqrl.Compile(myTemplate)
//Returns an anonymous function:
/*
function anonymous(options, Sqrl) {
var tmpltRes='Hi, my name is ';tmpltRes+=Sqrl.F.e(options.name);
return tmpltRes
}*/
//This function can be called with options and Sqrl (Sqrl so that it can
//access helpers and filters) and will return the rendered template.

compiled({name: "Johnny Appleseed"}, Sqrl)
//Returns "Hi, my name is Johnny Appleseed"
```


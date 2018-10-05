---
description: The syntax of Sqrl.Render
---

# Render

## Syntax

```text
Sqrl.Render(template, options)
//If template is a function, returns the result of template(options, Sqrl)
//If template is a string, it will Compile the string
//and then return compiled(options, Sqrl)
```

{% hint style="info" %}
Rendering a function is usually better for performance, since Squirrelly doesn't have to re-compile the template each time it Renders.
{% endhint %}

{% hint style="info" %}
Caching is coming soon!
{% endhint %}

## Examples

### Rendering a string

```text
var myTemplate = `
My favorite template engine is {{fav}}
`
Sqrl.Render(myTemplate, {
    fav: "Squirrelly!"
})
//Returns "My favorite template engine is Squirrelly!"
```

### Rendering a function

```text
var myTemplate = `
My favorite template engine is {{fav}}
`
var compiledTemplate = Sqrl.Compile(myTemplate)
Sqrl.Render(compiledTemplate, {
    fav: "Squirrelly!"
})
//Returns "My favorite template engine is Squirrelly!"
```




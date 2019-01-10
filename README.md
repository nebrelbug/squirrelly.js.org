# Overview

Squirrelly is a template engine written in JavaScript.

With Squirrelly, you can write templates that are blazing fast and can be rendered in milliseconds, server-side or client-side.

Squirrelly doesn't just limit you to HTML--you can use it with any language, and custom delimeters make it so there aren't parsing errors. It's also tiny \(**~2.5 KB gzipped**\), has **0 dependencies**, and is **blazing fast**.

![](https://img.shields.io/bundlephobia/minzip/squirrelly.svg)

{% hint style="info" %}
Did you know that Squirrelly is consistently faster than most other template engines, according to benchmarks?
{% endhint %}

### Simple Template:

```text
var myTemplate = "<p>My favorite kind of cake is: {{favoriteCake}}</p>"

Sqrl.Render(myTemplate, {favoriteCake: 'Chocolate!'})
// Returns: '<p>My favorite kind of cake is: Chocolate!</p>
```

### Conditionals:

```text
{{if(options.somevalue === 1)}}
Display this
{{#else}}
Display this
{{/if}}
```

### Loops

```text
{{each(options.somearray)}}
Display this
The current array element is {{@this}}
The current index is {{@index}}
{{/each}}
```


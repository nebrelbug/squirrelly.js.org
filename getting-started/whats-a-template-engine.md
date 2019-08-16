# What's a template engine?

A template engine is a program that takes a template and data, and returns the template filled with the data. 

Many template engines work by turning the template into a function where one of the parameters is the data. This function can be cached and saved, so the template engine doesn't need to re-parse the template again.

## Example

```javascript
var template = "My favorite template engine is {{engine}}"
Sqrl.Render(template, {engine: 'Squirrelly'})
// My favorite template engine is Squirrelly
Sqrl.Render(template, {engine: 'not Dust'})
// My favorite template engine is not Dust
```


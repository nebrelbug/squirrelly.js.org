# Filters

## Basic Syntax

```text
{{somereference|somefilter|anotherfilter}}
```

Squirrelly has a filter syntax similar to Nunjucks or Swig. Just put a `|` and then the filter name. You can pipe a reference to multiple filters if you want.

{% hint style="info" %}
Remember, to use a filter, you must have defined it first. Learn how to define a filter [here](../api/definefilter.md)
{% endhint %}


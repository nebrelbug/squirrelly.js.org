# Native Helpers

A **native helper** is a helper that is turned into JavaScript code at compilation time, rather than being called at runtime. For example,

```text
{{log("hi")/}}
```

is turned into `console.log("hi")` . 

{% hint style="info" %}
Learn how to create your own native helpers [here](../api/definenativehelper.md)
{% endhint %}

## Examples

```text
{{log("hi")/}}
```

is turned into `console.log("hi")` . 




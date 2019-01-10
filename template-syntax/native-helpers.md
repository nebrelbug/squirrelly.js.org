# Native Helpers

A **native helper** is a helper that is turned into other JavaScript code, rather than being called at runtime. For example,

```text
{{log("hi")/}}
```

is turned into `console.log("hi")` . 

You can define your own native helpers too: learn [here](../api/definenativehelper.md).

## Examples

```text
{{log("hi")/}}
```

is turned into `console.log("hi")` . 




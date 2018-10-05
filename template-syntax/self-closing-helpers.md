---
description: Self-closing helper syntax in Squirrelly
---

# Self-Closing Helpers

## Basic Syntax

```text
{{helpername(params)/}}
```

## Examples

```text
{{log("Hi! The index is: " + @index)/}}
```

The `log` helper is a native, self-closing helper that's built in to Squirrelly. It turns into a `console.log` function that logs to the console every time the template is rendered.

{% hint style="info" %}
The `log`helper can be very useful for debugging.
{% endhint %}




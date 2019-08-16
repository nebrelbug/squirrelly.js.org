# Partials

{% hint style="info" %}
Remember that before including a Partial, you have to define it as explained [here](../api/definepartial.md).
{% endhint %}

Use the `include` native helper to include a partial you have previously defined in your template.

## Example

```text
{{include("mypartial")/}}
OR
{{include(mypartial)/}}
OR
{{include('mypartial')/}}
```




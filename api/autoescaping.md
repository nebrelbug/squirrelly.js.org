# autoEscaping

Auto-Escaping is an important feature of Squirrelly. When it's enabled, every reference without the `safe` filter will be HTML-escaped, to provide some protection against XSS.

```text
Sqrl.autoEscaping(true) // Turns autoEscaping on
Sqrl.autoEscaping(false) // Turns autoEscaping off
// autoEscaping is on by default
```

{% hint style="info" %}
Auto-escaping can be helpful, but it also negatively impacts performance. For best results, autoEscape data before you store it or attempt to render it in a template.
{% endhint %}


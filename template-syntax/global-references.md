---
description: Global reference syntax in Squirrelly
---

# Global References

In Squirrelly, a reference is a single value that's passed in as an option to the template. There are two types of references, global references and [helper references](helper-references.md).

## Basic syntax:

```text
<p>This is a global reference: {{myname}}</p>
```

Put a global reference between the opening and closing delimeters \(by default `{{`and `}}`.

Global references are always in the global scope, and can be written anywhere in your code. Since Squirrelly templates parse into JavaScript, you can write a reference like this: `<p>This is the child of an object: {{user.lastName}}`

or like this:

`<p>This is the child of an object: {{user['lastName']}}`.

{% hint style="warning" %}
There can be spaces after the beginning bracket and before the closing bracket, but any reference that doesn't point to an actual value, like`{{hi people}},` will make your code break!
{% endhint %}


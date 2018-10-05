---
description: Helper reference syntax in Squirrelly
---

# Helper References

In Squirrelly, a reference is a single value that's passed in as an option to the template. There are two types of references, [global references ](global-references.md)and helper references.

A helper reference is a reference that points to data created by a helper. For example, when looping through an object using the `foreach` helper

## Basic syntax {#basic-syntax}

```text
<p>This is a helper reference: {{@stuff}}</p>
```

Prefix a helper reference with `@`. 

Helper references are always in the scope of its parent helper.

## Scoping

After the `@`, place one `../` for each level of helper you want to go back. If you specified an id when you created the helper:

```text
{{helper(params) someid}}
{{/helper}}
```

Then you can reference that helper like this: `{{@someid:helperref}}`


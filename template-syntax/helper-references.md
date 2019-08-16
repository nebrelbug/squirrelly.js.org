# Helper References

In Squirrelly, a reference is a single value that's passed in as an option to the template. There are two types of references, [global references ](global-references.md)and helper references.

A helper reference is a reference that points to data created by a helper. For example, when looping through an object using the `foreach` helper

## Basic syntax <a id="basic-syntax"></a>

```text
<p>This is a helper reference: {{@stuff}}</p>
```

Prefix a helper reference with `@`. 

Helper references are always in the scope of its parent helper.

## Scoping

To access the helper references of an outside helper, you can use scoping. Example:

```text
{{helper1(parameters)}}
Do this
{{helper2(parameters)}}
This is a helper ref from helper2: {{@someref}}
This is a helper ref from helper1: {{@../someref}}
{{/helper2}}
{{/helper1}}
```

## ID

If you have many layers of nestedness, it can be easier to use ID's instead of scoping.

```text
{{helper1(parameters) someID}}
Do this
{{helper2(parameters)}}
This is a helper ref from helper2: {{@someref}}
This is a helper ref from helper1: {{@someID:someref}}
{{/helper2}}
{{/helper1}}
```


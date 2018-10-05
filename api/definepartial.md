---
description: A guide to using Partials in Squirrelly
---

# definePartial

```text
Sqrl.definePartial("mypartial", `
This is a partial.
It can be called with the data of the template it's in.
`)
```

Then to use the partial in your template:

```text
{{include("mypartial")/}}
OR
{{include(mypartial)/}}
OR
{{include('mypartial')/}}
```


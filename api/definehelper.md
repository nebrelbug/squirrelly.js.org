---
description: The syntax of Sqrl.defineHelper
---

# defineHelper

```text
Sqrl.defineHelper("helperName", function(args, content, blocks, options) {
    //Do whatever you want here with the arguments, blocks, and content
    //Example:
    return "Wrapper: " + blocks.date() + "Wrapper"
})
```


# defineHelper

```text
Sqrl.defineHelper("helperName", function(args, content, blocks) {
    //Do whatever you want here with the arguments, blocks, and content
    //Example:
    return "Wrapper: " + blocks.date() + "Wrapper"
})
```

### Parameters

`args`: contains the arguments passed to the function.

`content`: is a function that can be called \(optionally, by passing in helper references\) and that returns the default content.

`blocks`: an object that contains each of the helper blocks, which are functions \(like `content` and are sorted by key.


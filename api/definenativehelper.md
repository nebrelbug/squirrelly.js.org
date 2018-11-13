# defineNativeHelper

```text
Sqrl.defineNativeHelper (name, obj)
// This is the code for the native 'if' helper
Sqrl.defineNativeHelper('if', {
    helperStart: function (param) { // helperStart is called with (params, id) but id isn't needed
      return 'if(' + param + '){'
    },
    helperEnd: function () {
      return '}'
    },
    blocks: {
      else: function () { // called with (id) but neither param is needed
        return '}else{'
      }
    }
})
```


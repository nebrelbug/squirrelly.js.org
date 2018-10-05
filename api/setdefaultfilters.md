---
description: The syntax of Sqrl.setDefaultFilters
---

# setDefaultFilters

```text
setDefaultFilters("clear") //This removes all default filters
setDefaultFilters({filtername: true}) //This sets the filter 'filtername'
//as a default filter
setDefaultFilters({filtername: true, otherfilter: true}) //This sets both
//'filtername' and 'otherfilter' to be default filters
setDefaultFilters({filtername: false}) //This makes 'filtername' not a
//default filter
```

Simply put, `setDefaultFilters` has one parameter. If the parameter is "clear" then `defaultFilters`  \(which isn't exposed to the user\) is set to `{}` . If the parameter is an object, then it loops over each property and sets it on `defaultFilters`.

When a reference is parsed, it is passed through the filters with the same name as the properties on `defaultFilters`, as long as it is set to `true`.


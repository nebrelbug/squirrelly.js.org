---
description: A list of all Squirrelly's built-in native helpers..
---

# Built-in Helpers

## if/else

```text
{{if(options.somevalue === 1)}}
Display this
{{#else}}
Display this
{{/if}}
```

## each

```text
{{each(options.somearray)}}
Display this
The current array element is {{@this}}
The current index is {{@index}}
{{/each}}
```

### Helper References:

* `this`: the current array element
* `index`: the index of the array element

## foreach

```text
{{foreach(options.someobject)}}
This loops over each of an objects keys and values.
The value of the current child is {{@this}}
The current key is {{@key}}
{{/foreach}}
```

### Helper References:

* `this`: the value of the current object child
* `key`: the key of the current child

## log

```text
{{log("The value of options.arr is: " + options.arr)/}}
```

{% hint style="info" %}
The log helper is a self-closing, native helper. It's turned into this code:

_console.log\("The value of options.arr is: " + options.arr\);_

The log helper can be extremely helpful for debugging.
{% endhint %}

## tags

```text
{{tags(--,--)/}}
--somevalue--
```

{% hint style="info" %}
Setting custom tags can be really helpful when writing in a language such as LaTek.
{% endhint %}

## js

```text
{{js(options.newvalue = options.oldvalue + 983 * 2)/}}
{{newvalue}}
```


# Why Squirrelly?

## Features

Squirrelly has a number of features that set it apart from the competition:

* It's faster than most templating engines
* It supports user-defined helpers and native helpers
* It supports filters
* It supports partials
* It supports custom tags \(delimeters\)
* It's incredibly lightweight: in comparison: the full version only weighs about **2.2 KB gzipped**, compared to Pug's **237 KB** and Handlebars' **21.5 KB**
* It works with other languages than HTML
* It's not white-space sensitive

| **Feature** | **Squirrelly** | Handlebars | Pug | Marko | Dust | Swig |
| :--- | :--- | :--- | :--- | :--- | :--- | :--- |
| Auto Escape |  ✓ |  ✓ |  ✓ |  ✓ |  ✓ |  ✓ |
| Whitespace sensitive | No | No | Yes | No | No | No |
| Content Type | All | All | HTML | HTML | All | All |

## Why Regular Expressions?

Though some people think that regular expressions aren't a good idea for template engines, we believe they're the right choice for Squirrelly because of the speed they allow, because of the extensive testing we've done, and because of the relative simplicity of Squirrelly's syntax.


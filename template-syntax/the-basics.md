# The Basics

## Language Items

There are 4 types of language items in Squirrelly:

* References \([global](global-references.md) and [helper](helper-references.md)\). These are references to the actual data of options that are passed in.
* [Helpers](https://stackedit.io/app#helpers). These are for logic in the template. Loops and conditionals are both implemented as native helpers, a special kind of helper that compiles into native JS code before rendering.
* [Filters](https://stackedit.io/app#filters). These are for processing a string after it’s been evaluated. Escaping and trimming are done with filters.

## Inspiration

Squirrelly takes inspiration from Mustache, Handlebars, Nunjucks, Swig, and many other great template engines.


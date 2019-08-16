---
description: Install Squirrelly
---

# Installation

## Node

```
npm install --save squirrelly
```

After the install is finished, accessing Squirrelly is as simple as:

```javascript
var Sqrl = require('squirrelly')
```

If you're using ES Modules, you can also do

```javascript
import * as Sqrl from 'squirrelly'
```

## With a CDN

All of the following methods make Squirrelly available through the global object `Sqrl`.

{% hint style="info" %}
If you need to compile templates in the browser, use the full version. For best performance, though, `Compile` your templates into functions first and include them in the JavaScript of your site, and include just the runtime.
{% endhint %}

### Full Version

#### Minified

```text
<script src="https://unpkg.com/squirrelly@latest/dist/squirrelly.min.js"></script>
```

#### Development

```text
<script src="https://unpkg.com/squirrelly@latest/dist/squirrelly.dev.js"></script>
```

### Runtime

#### Minified

```text
<script src="https://unpkg.com/squirrelly@latest/dist/squirrelly.runtime.js"></script>
```

#### Development

```text
<script src="https://unpkg.com/squirrelly@latest/dist/squirrelly.runtime.dev.js"></script
```


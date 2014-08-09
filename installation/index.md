title: How to install
description: functional.js works in the browser and with node.js, there are several options for installation.
---

## Node.js

### Install

Install via npm and save the dependency in your package.json:

```bash
npm install functional.js --save
```

Then to include functional.min.js in your app:

```js
var fjs = require("functional.js");
```

### Update

```bash
npm update functional.js
```

## Client side

### Direct include

There is no CDN yet, you should download the latest minified version from [here](http://bit.ly/funcmin) and host it yourself. Once you reference the js file "fjs" will become a global variable.

### Bower

```bash
bower install functional.js
```

## Source code

The source code is available on [Github](https://github.com/leecrossley/functional-js), you can clone the repo:

```bash
git clone git@github.com:leecrossley/functional-js.git
```

title: fjs.apply function to items
description: fjs.apply maps internal function results to a new array.
---

## fjs.apply

fjs.apply is a special kind of fjs.map that applies a function available to all the items in the list and returns a new array with the results.

### Usage

```js
fjs.apply(functionName, items);
```

### Basic example

```js
var applyCase = fjs.apply("toUpperCase");

applyCase(["Hello", "World"]);
// => ["HELLO", "WORLD"]
```

### Multiple argument example

```js
var applyIndexOf = fjs.apply(["substring", "1", "4"]);

applyIndexOf(["Hello", "World"]);
// => ["ell", "orl"];
```

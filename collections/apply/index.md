title: λ.apply function to items
description: λ.apply maps internal function results to a new array.
---

## λ.apply

λ.apply is a special kind of λ.map that applies a function available to all the items in the list and returns a new array with the results.

### Usage

```js
λ.apply(functionName, items);
```

### Basic example

```js
var applyCase = λ.apply("toUpperCase");

applyCase(["Hello", "World"]);
// => ["HELLO", "WORLD"]
```

### Multiple argument example

```js
var applyIndexOf = λ.apply(["substring", "1", "4"]);

applyIndexOf(["Hello", "World"]);
// => ["ell", "orl"];
```

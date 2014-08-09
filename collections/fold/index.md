title: fold array to value with fjs.fold
description: fjs.fold is similar to fjs.reduce but takes an initial value.
---

## fjs.fold

- *Alias:* fjs.foldl

fjs.fold is similar to [fjs.reduce](/collections/reduce/) but takes an initial value. It supports currying by default.

### Usage

```js
fjs.fold(iterator, initial, items);
```

### Example

```js
var multiply = function (arg1, arg2) {
    return arg1 * arg2;
};

var multiplyFoldFrom10 = fjs.fold(multiply, 10);

multiplyFoldFrom10([1, 2, 3]); // => 60
```

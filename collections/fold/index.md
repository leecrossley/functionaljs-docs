title: fold array to value with λ.fold
description: λ.fold is similar to λ.reduce but takes an initial value.
---

## λ.fold

- *Alias:* λ.foldl

λ.fold is similar to [λ.reduce](/collections/reduce/) but takes an initial value. It supports currying by default.

### Usage

```js
λ.fold(iterator, initial, items);
```

### Example

```js
var multiply = function (arg1, arg2) {
    return arg1 * arg2;
};

var multiplyFoldFrom10 = λ.fold(multiply, 10);

multiplyFoldFrom10([1, 2, 3]); // => 60
```

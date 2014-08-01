title: Reduce array to value with λ.reduce
description: λ.reduce applies an iterator function against an internal accumulator object and all items in the list are reduced to a single value.
---

## λ.reduce

- *Alias:* λ.reducel
- *Alias:* λ.foldll

λ.reduce applies an iterator function against an internal accumulator object and all items in the list are reduced to a single value. Similar to the native Array.prototype.reduce() available in ES5 but does not use any native functions and supports currying by default (as well as working in older browsers).

### Usage

```js
λ.reduce(iterator, items);
```

### Example

```js
var multiply = function (arg1, arg2) {
    return arg1 * arg2;
};

var multiplyReduce = λ.reduce(multiply);

multiplyReduce([1, 2, 3]); // => 6
```

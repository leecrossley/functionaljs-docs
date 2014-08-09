title: Reduce array to value with fjs.reduce
description: fjs.reduce applies an iterator function against an internal accumulator object and all items in the list are reduced to a single value.
---

## fjs.reduce

- *Alias:* fjs.reducel
- *Alias:* fjs.foldll

fjs.reduce applies an iterator function against an internal accumulator object and all items in the list are reduced to a single value. Similar to the native Array.prototype.reduce() available in ES5 but does not use any native functions and supports currying by default (as well as working in older browsers).

### Usage

```js
fjs.reduce(iterator, items);
```

### Example

```js
var multiply = function (arg1, arg2) {
    return arg1 * arg2;
};

var multiplyReduce = fjs.reduce(multiply);

multiplyReduce([1, 2, 3]); // => 6
```

title: Simply the fjs.best item
description: fjs.best returns the best item in an array based on the return value for the iterator function.
---

## fjs.best

fjs.best returns the *best* item in a list based on the return value for the iterator function - it's essentially a special fjs.reduce. Can be curried by default.

### Usage

```js
fjs.best(iterator, items);
```

### Example

```js
var longest = fjs.best(function (arg1, arg2) {
    return arg1.length > arg2.length;
});

longest(["simply", "the", "best"]); // => "simply"
```

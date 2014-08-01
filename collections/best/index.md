title: Simply the λ.best item
description: λ.best returns the best item in an array based on the return value for the iterator function.
---

## λ.best

λ.best returns the *best* item in a list based on the return value for the iterator function - it's essentially a special λ.reduce. Can be curried by default.

### Usage

```js
λ.best(iterator, items);
```

### Example

```js
var longest = λ.best(function (arg1, arg2) {
    return arg1.length > arg2.length;
});

longest(["simply", "the", "best"]); // => "simply"
```

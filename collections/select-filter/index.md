title: λ.select items that match condition
description: λ.select returns a new array with all elements that return true for the iterator function.
---

## λ.select

- *Alias:* λ.filter

λ.select returns a new array with all items that return true for the iterator function. Can be curried by default.

### Usage

```js
λ.select(iterator, items);
```

### Example

```js
var even = function (item) {
    return item % 2 === 0;
};
var odd = function (item) {
    return item % 2 !== 0;
};

var selectEven = λ.select(even);
var selectOdd = λ.select(odd);

selectEven([1, 2, 3, 4, 5]); // => [2, 4]
selectOdd([1, 2, 3, 4, 5]); // => [1, 3, 5]
```

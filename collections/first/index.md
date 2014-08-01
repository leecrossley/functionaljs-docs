title: λ.first in array
description: λ.first returns the first item in a list that returns true for the iterator function.
---

## λ.first

λ.first returns the first item in a list that returns true for the iterator function. Can be curried by default.

### Usage

```js
λ.first(iterator, items);
```

### Example

```js
var even = function (item) {
    return item % 2 === 0;
};
var odd = function (item) {
    return item % 2 !== 0;
};

var firstEven = λ.first(even);
var firstOdd = λ.first(odd);

firstEven([5, 4, 3, 2, 1]); // => 4
firstOdd([5, 4, 3, 2, 1]); // => 5
```

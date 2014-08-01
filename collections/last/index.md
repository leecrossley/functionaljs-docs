title: λ.last in array
description: λ.last returns the last item in a list that returns true for the iterator function.
---

## λ.last

λ.last returns the last item in a list that returns true for the iterator function. Can be curried by default.

### Usage

```js
λ.last(iterator, items);
```

### Example

```js
var even = function (item) {
    return item % 2 === 0;
};
var odd = function (item) {
    return item % 2 !== 0;
};

var lastEven = λ.last(even);
var lastOdd = λ.last(odd);

lastEven([5, 4, 3, 2, 1]); // => 2
lastOdd([5, 4, 3, 2, 1]); // => 1
```

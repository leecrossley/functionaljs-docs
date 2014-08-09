title: fjs.last in array
description: fjs.last returns the last item in a list that returns true for the iterator function.
---

## fjs.last

fjs.last returns the last item in a list that returns true for the iterator function. Can be curried by default.

### Usage

```js
fjs.last(iterator, items);
```

### Example

```js
var even = function (item) {
    return item % 2 === 0;
};
var odd = function (item) {
    return item % 2 !== 0;
};

var lastEven = fjs.last(even);
var lastOdd = fjs.last(odd);

lastEven([5, 4, 3, 2, 1]); // => 2
lastOdd([5, 4, 3, 2, 1]); // => 1
```

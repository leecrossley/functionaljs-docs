title: λ.partition items in array
description: λ.partition returns an array of two arrays (first array is all items that return true)
---

## λ.partition

λ.partition returns an array of two arrays. The first array is all items that return true for the iterator function, the second array is all items that return false for the iterator function (i.e. the rest).

### Usage

```js
λ.partition(iterator, items);
```

### Example

```js
var even = function (item) {
    return item % 2 === 0;
};

var partitionEven = λ.partition(even);

partitionEven([7, 6, 5, 4, 3, 2, 1]);
// => [[6, 4, 2], [7, 5, 3, 1]]
```

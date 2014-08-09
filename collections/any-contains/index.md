title: fjs.any item in array
description: fjs.any will return true if an item is present in the list.
---

## fjs.any

- *Alias:* fjs.contains

fjs.any will return true if an item is present in the list that returns true when passed to the iterator function. This is different from "indexOf" that looks up items in arrays without an iterator function.

### Usage

```js
fjs.any(iterator, items);
```

### Example

```js
var even = function (item) {
    return item % 2 === 0;
};

var anyEven = fjs.any(even);

anyEven([1, 2, 3]); // => true
anyEven([1, 3, 5]); // => false
```

title: λ.any item in array
description: λ.any will return true if an item is present in the list.
---

## λ.any

- *Alias:* λ.contains

λ.any will return true if an item is present in the list that returns true when passed to the iterator function. This is different from "indexOf" that looks up items in arrays without an iterator function.

### Usage

```js
λ.any(iterator, items);
```

### Example

```js
var even = function (item) {
    return item % 2 === 0;
};

var anyEven = λ.any(even);

anyEven([1, 2, 3]); // => true
anyEven([1, 3, 5]); // => false
```

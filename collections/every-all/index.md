title: λ.every item in array
description: λ.every tests whether all items in the list pass the test implemented by the iterator function.
---

## λ.every

- *Alias:* λ.all

λ.every will return true if all the items in the list return true when passed to the iterator function individually, otherwise it will return false. λ.every be curried by default.

### Usage

```js
λ.every(iterator, items);
```

### Example

```js
var even = function (item) {
    return item % 2 === 0;
};
var odd = function (item) {
    return item % 2 !== 0;
};

var everyEven = λ.every(even);
var everyOdd = λ.every(odd);

everyEven([2, 4, 6, 8]); // => true
everyOdd([1, 3, 6, 9]); // => false
```

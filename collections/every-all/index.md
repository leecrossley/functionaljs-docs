title: fjs.every item in array
description: fjs.every tests whether all items in the list pass the test implemented by the iterator function.
---

## fjs.every

- *Alias:* fjs.all

fjs.every will return true if all the items in the list return true when passed to the iterator function individually, otherwise it will return false. fjs.every be curried by default.

### Usage

```js
fjs.every(iterator, items);
```

### Example

```js
var even = function (item) {
    return item % 2 === 0;
};
var odd = function (item) {
    return item % 2 !== 0;
};

var everyEven = fjs.every(even);
var everyOdd = fjs.every(odd);

everyEven([2, 4, 6, 8]); // => true
everyOdd([1, 3, 6, 9]); // => false
```

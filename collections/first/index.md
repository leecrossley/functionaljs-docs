title: fjs.first in array
description: fjs.first returns the first item in a list that returns true for the iterator function.
---

## fjs.first

- *Alias:* fjs.head
- *Alias:* fjs.take

fjs.first returns the first item in a list that returns true for the iterator function. Can be curried by default.

### Usage

```js
fjs.first(iterator, items);
```

### Example

```js
var even = function (item) {
    return item % 2 === 0;
};
var odd = function (item) {
    return item % 2 !== 0;
};

var firstEven = fjs.first(even);
var firstOdd = fjs.first(odd);

firstEven([5, 4, 3, 2, 1]); // => 4
firstOdd([5, 4, 3, 2, 1]); // => 5
```

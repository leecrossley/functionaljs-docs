title: fjs.rest in array
description: fjs.rest returns the rest of the items in a list that return true for the iterator function.
---

## fjs.rest

- *Alias:* fjs.tail
- *Alias:* fjs.drop

fjs.rest returns the rest of the items in a list that return true for the iterator function. Can be curried by default.

### Usage

```js
fjs.rest(iterator, items);
```

### Example

```js
var even = function (item) {
    return item % 2 === 0;
};
var odd = function (item) {
    return item % 2 !== 0;
};

var restEven = fjs.rest(even);
var restOdd = fjs.rest(odd);

restEven([5, 4, 3, 2, 1]); // => [2]
restOdd([5, 4, 3, 2, 1]); // => [3, 1]
```

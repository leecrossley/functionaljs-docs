title: Select from array while
description: fjs.while returns items from an array while the iterator function returns true.
---

## fjs.while

fjs.while returns items from an array while the iterator function returns true. Unlike [fjs.select](/collections/select-filter/), this function limits the  returned array to the first item that evaluates false. Can be curried by default.

### Usage

```js
fjs.while(iterator, items);
```

### Example

```js
var whileEven = fjs.while(function (item) {
    return item % 2 === 0;
});

whileEven([2, 4, 5, 6]); // => [2, 4]
```

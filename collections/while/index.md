title: Select from array while
description: λ.while returns items from an array while the iterator function returns true.
---

## λ.while

λ.while returns items from an array while the iterator function returns true. Unlike [λ.select](/collections/select-filter/), this function limits the  returned array to the first item that evaluates false. Can be curried by default.

### Usage

```js
λ.while(iterator, items);
```

### Example

```js
var whileEven = λ.while(function (item) {
    return item % 2 === 0;
});

whileEven([2, 4, 5, 6]); // => [2, 4]
```

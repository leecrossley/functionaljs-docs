title: Map array items with fjs.map
description: fjs.map allows iteration over a list of items, applying an iterator function to each and returns a new array with the yielded values.
---

## fjs.map

fjs.map allows iteration over a list of items, applying an iterator function to each and returning a new array with the yielded values. This is similar to the native map function available in modern browsers but uses its own implementation that utilises fjs.curry by default.

### Usage

```js
fjs.map(iterator, items);
```

### Example

```js
var items = [1, 2, 3];

var doubleUp = function (number) {
    return number * 2;
};

var doubleMap = fjs.map(doubleUp);

doubleMap(items);
// => [2, 4, 6];
```

"doubleUp" is the iterator function applied to each item in the list ("items" array). "doubleMap" is a higher order function created by partially invoking "doubleUp".

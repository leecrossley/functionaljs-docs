title: Unique items from array (nub)
description: fjs.nub returns items from an array while the iterator function returns true.
---

## fjs.nub

- *Alias:* fjs.unique
- *Alias:* fjs.distinct

fjs.nub removes duplicate elements from a list and returns a new array containing only unique elements, specifically the first of each duplicate element found in the list. Function takes a comparator that determines equality (uniqueness) and the list to run the function against. Can be curried by default.

### Usage

```js
fjs.nub(iterator, items);
```

### Example

```js
var unique = fjs.nub(function (arg1, arg2) {
    return arg1 === arg2;
});

unique(["John", "Jane", "Jane", "Jane", "Joe", "John"]);
// => ["John", "Jane", "Joe"]
```

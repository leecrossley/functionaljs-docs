title: Unique items from array (nub)
description: fjs.nub returns items from an array that are unique.
---

## fjs.nub

- *Alias:* fjs.unique
- *Alias:* fjs.distinct

fjs.nub removes duplicate elements from a list and returns a new array containing only the unique elements. fjs.nub takes an iterator function and a list to apply the iterator to. The iterator function takes two given elements from the list and determines if they are the same, and therefore unique, or not.  Can be curried by default.

### Usage

```js
fjs.nub(comparator, items);
```

### Example

```js
var unique = fjs.nub(function (arg1, arg2) {
    return arg1 === arg2;
});

unique(["John", "Jane", "Jane", "Jane", "Joe", "John"]);
// => ["John", "Jane", "Joe"]
```

fjs.nub returns only the first unique element found in a list. This behavior is more apparent when applied to a list of more complex objects.


### Another Example

```js
var unique = fjs.nub(function (arg1, arg2) {
	return arg1.valueA === arg2.valueA;
});

unique([{valueA: 1, valueB: 2},{valueA: 2, valueB: 3},{valueA: 1, valueB: 3},{valueA: 1, valueB: 4}]);
// => [{valueA: 1, valueB: 2},{valueA: 2, valueB: 3}];
```
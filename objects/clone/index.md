title: fjs.clone an array
description: fjs.clone returns a copy of an array.
---

## fjs.clone

fjs.clone returns a copy of an array. Useful if you want to manipulate an array without modifying the original, such as with the native "reverse" function.

### Usage

```js
fjs.clone(items);
```

### Example

```js
fjs.clone([5, 4, 3, 2, 1]); // => [5, 4, 3, 2, 1]
```

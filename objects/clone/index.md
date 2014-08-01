title: λ.clone an array
description: λ.clone returns a copy of an array.
---

## λ.clone

λ.clone returns a copy of an array. Useful if you want to manipulate an array without modifying the original, such as with the native "reverse" function.

### Usage

```js
λ.clone(items);
```

### Example

```js
λ.clone([5, 4, 3, 2, 1]); // => [5, 4, 3, 2, 1]
```

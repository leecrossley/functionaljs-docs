title: Convert object fjs.toArray
description: fjs.toArray converts an object with properties to an array.
---

## fjs.toArray

fjs.toArray converts an object with properties to an array.

### Usage

```js
fjs.toArray(obj);
```

### Example

```js
var obj = {
    "p1": "abc",
    "p2": false,
    "p3": null
};

fjs.toArray(obj);
// => [["p1", "abc"], ["p2", false], ["p3", null]]
```

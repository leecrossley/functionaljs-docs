title: Convert object λ.toArray
description: λ.toArray converts an object with properties to an array.
---

## λ.toArray

λ.toArray converts an object with properties to an array.

### Usage

```js
λ.toArray(obj);
```

### Example

```js
var obj = {
    "p1": "abc",
    "p2": false,
    "p3": null
};

λ.toArray(obj);
// => [["p1", "abc"], ["p2", false], ["p3", null]]
```

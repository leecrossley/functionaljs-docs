title: λ.truthy object
description: λ.truthy returns true if an object can be coerced to true in a boolean context.
---

## λ.truthy

λ.truthy returns true if an object can be coerced to true in a boolean context.

### Usage

```js
λ.truthy(obj);
```

### Examples

```js
expect(λ.truthy(false); // => false
expect(λ.truthy(null); // => false

expect(λ.truthy(true); // => true
expect(λ.truthy("abc"); // => true
```

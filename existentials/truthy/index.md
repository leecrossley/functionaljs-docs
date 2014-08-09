title: fjs.truthy object
description: fjs.truthy returns true if an object can be coerced to true in a boolean context.
---

## fjs.truthy

fjs.truthy returns true if an object can be coerced to true in a boolean context.

### Usage

```js
fjs.truthy(obj);
```

### Examples

```js
expect(fjs.truthy(false); // => false
expect(fjs.truthy(null); // => false

expect(fjs.truthy(true); // => true
expect(fjs.truthy("abc"); // => true
```

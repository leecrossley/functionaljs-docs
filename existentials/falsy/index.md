title: λ.falsy object
description: λ.falsy returns true if an object can be coerced to false in a boolean context.
---

## λ.falsy

λ.falsy returns true if an object can be coerced to false in a boolean context.

### Usage

```js
λ.falsy(obj);
```

### Examples

```js
expect(λ.falsy(false); // => true
expect(λ.falsy(null); // => true

expect(λ.falsy(true); // => false
expect(λ.falsy("abc"); // => false
```

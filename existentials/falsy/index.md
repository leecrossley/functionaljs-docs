title: fjs.falsy object
description: fjs.falsy returns true if an object can be coerced to false in a boolean context.
---

## fjs.falsy

fjs.falsy returns true if an object can be coerced to false in a boolean context.

### Usage

```js
fjs.falsy(obj);
```

### Examples

```js
expect(fjs.falsy(false); // => true
expect(fjs.falsy(null); // => true

expect(fjs.falsy(true); // => false
expect(fjs.falsy("abc"); // => false
```

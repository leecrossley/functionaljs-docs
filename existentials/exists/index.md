title: λ.exists (not null or undefined)
description: λ.exists returns false if an object is null or undefined.
---

## λ.exists

λ.exists returns false if an object is null or undefined (considered not to exist), all other values return true.
### Usage

```js
λ.exists(obj);
```

### Examples

```js
λ.exists(undefined); // => false
λ.exists(null); // => false

λ.exists(1); // => true
λ.exists("abc"); // => true
```

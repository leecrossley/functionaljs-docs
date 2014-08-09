title: fjs.exists (not null or undefined)
description: fjs.exists returns false if an object is null or undefined.
---

## fjs.exists

fjs.exists returns false if an object is null or undefined (considered not to exist), all other values return true.
### Usage

```js
fjs.exists(obj);
```

### Examples

```js
fjs.exists(undefined); // => false
fjs.exists(null); // => false

fjs.exists(1); // => true
fjs.exists("abc"); // => true
```

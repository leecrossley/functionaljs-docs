title: Object λ.isFunction
description: λ.isFunction returns true if the object is a function, otherwise false.
---

## λ.isFunction

λ.isFunction returns true if the object is a function, otherwise false.

### Usage

```js
λ.isFunction(obj);
```

### Example

```js
λ.isFunction(λ.reduce(function (arg1, arg2) {
    return arg1 * arg2;
})); // => true
```

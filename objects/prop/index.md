title: fjs.prop object property
description: fjs.prop returns a function that will return the value of any property name argument.
---

## fjs.prop

fjs.prop returns a function that will return the value of any property name argument.

### Usage

```js
fjs.prop(propertyName);
```

### Example

```js
fjs.prop("hello")({ "hello": "world" }); // => "world"
```

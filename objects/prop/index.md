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

{% note warn Implementation issue %}
This implementation is under consideration to be rewritten, inline with other functions that can already be curried in the standard way.
{% endnote %}

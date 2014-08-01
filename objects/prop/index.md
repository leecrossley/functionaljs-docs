title: λ.prop object property
description: λ.prop returns a function that will return the value of any property name argument.
---

## λ.prop

λ.prop returns a function that will return the value of any property name argument.

### Usage

```js
λ.prop(propertyName);
```

### Example

```js
λ.prop("hello")({ "hello": "world" }); // => "world"
```

{% note warn Implementation issue %}
This implementation is under consideration to be rewritten, inline with other functions that can already be curried in the standard way.
{% endnote %}

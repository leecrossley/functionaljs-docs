title: λ.pluck a property
description: λ.pluck maps / extracts a list of property values from items in an array.
---

## λ.pluck

λ.pluck is a special kind of λ.map that extracts a list of property values for a given property name from items in an array.

### Usage

```js
λ.pluck(propertyName, items);
```

{% note info Implementation note %}
It is worth noting that this implementation is the same as λ.map(λ.prop(propertyName), items);
{% endnote %}

### Basic example

```js
var items = [{
    "p1": "abc",
    "p2": 123
}, {
    "p1": "cab",
    "p2": 312
},{
    "p1": "bca",
    "p2": 231
}];

var pluck1 = λ.pluck("p1");

pluck1(items);
// => ["abc", "cab", "bca"]
```

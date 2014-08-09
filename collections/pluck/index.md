title: fjs.pluck a property
description: fjs.pluck maps / extracts a list of property values from items in an array.
---

## fjs.pluck

fjs.pluck is a special kind of fjs.map that extracts a list of property values for a given property name from items in an array.

### Usage

```js
fjs.pluck(propertyName, items);
```

{% note info Implementation note %}
It is worth noting that this implementation is the same as fjs.map(fjs.prop(propertyName), items);
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

var pluck1 = fjs.pluck("p1");

pluck1(items);
// => ["abc", "cab", "bca"]
```

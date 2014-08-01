title: Iterate items with λ.each
description: λ.each allows iteration over a list of items, applying an iterator function to each item.
---

## λ.each

λ.each allows iteration over a list of items, applying an iterator function to each item. This is similar to the native forEach function available in modern browsers but uses its own implementation that utilises λ.curry by default.

### Usage

```js
λ.each(iterator, items);
```

### Example

```js
var result = [];
var items = ["f", "u", "n", "c"];

var addTo = function (item) {
    return result.push(item);
};

var addToResult = λ.each(addTo);

addToResult(items);
// => ["f", "u", "n", "c"]
```

"addTo" is the iterator function applied to each item in the list ("items" array). "addToResult" is a higher order function created by partially invoking the "addTo". The "addToResult" function can be reused with different arrays if required.

{% note warn Breaking out %}
You cannot "break;" from an λ.each, it is intended to always iterate for all items. Other functions do allow breaking out of loops and achieve similar results.
{% endnote %}

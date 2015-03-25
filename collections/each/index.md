title: Iterate items with fjs.each
description: fjs.each allows iteration over a list of items, applying an iterator function to each item.
---

## fjs.each

fjs.each allows iteration over a list of items, applying an iterator function to each item. This is similar to the native forEach function available in modern browsers but uses its own implementation that utilises fjs.curry by default.

### Usage

```js
fjs.each(iterator, items);
```

### Example

```js
var result = [];
var items = ["f", "u", "n", "c"];

var addTo = function (item) {
    return result.push(item);
};

var addToResult = fjs.each(addTo);

addToResult(items);
// => ["f", "u", "n", "c"]
```

"addTo" is the iterator function applied to each item in the list ("items" array). "addToResult" is a higher order function created by partially invoking the "addTo". The "addToResult" function can be reused with different arrays if required.

{% note warn Breaking out %}
You cannot "break;" from an fjs.each, it is intended to always iterate for all items. Other functions do allow breaking out of loops and achieve similar results.
{% endnote %}

## Implicit index

fjs.each will provide your iterator function with the index in an optional second parameter.

### Example

```js
var result = [];
var items = ["f", "u", "n", "c"];

var addTo = function (item, i) {
    return result.push({
        "index": i,
        "item": item});
    };

    var addToResult = fjs.each(addTo);

    addToResult(items);
    // => [{ "index": 0, "item": "f" } ,{ "index": 1, "item": "u" }, { "index": 2, "item": "n" }, { "index": 3, "item": "c" }]
    ```

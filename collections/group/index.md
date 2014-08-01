title: λ.group items in array
description: λ.group returns an object with items grouped by a property
---

## λ.group

λ.group returns an object with items grouped by a property, determined by the iterator function. Can be curried by default.

### Usage

```js
λ.group(iterator, items);
```

### Example

```js
var groupByFirstLetter = λ.group(function (item) {
    return item.charAt(0);
};

groupByFirstLetter(["Lee", "Ryan", "Leona", "Sarah", "Rob", "Liam"]);
// => {"L": [ "Lee", "Leona", "Liam" ], "R": [ "Ryan", "Rob" ], "S": [ "Sarah" ]}
```

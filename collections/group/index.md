title: fjs.group items in array
description: fjs.group returns an object with items grouped by a property
---

## fjs.group

fjs.group returns an object with items grouped by a property, determined by the iterator function. Can be curried by default.

### Usage

```js
fjs.group(iterator, items);
```

### Example

```js
var groupByFirstLetter = fjs.group(function (item) {
    return item.charAt(0);
};

groupByFirstLetter(["Lee", "Ryan", "Leona", "Sarah", "Rob", "Liam"]);
// => {"L": [ "Lee", "Leona", "Liam" ], "R": [ "Ryan", "Rob" ], "S": [ "Sarah" ]}
```

title: fjs.assign object properties
description: fjs.assign extends/assigns all the properties in the source object(s) to the destination object.
---

## fjs.assign

- *Alias:* fjs.extend

fjs.assign extends/assigns all the properties in the source object(s) to the destination object and returns the destination object. Can be curried by default.

### Usage

```js
fjs.assign(obj1, obj2);
```

### Basic example

```js
var obj1 = {
    prop1: "obj1prop1",
    prop2: "obj1prop2"
};
var obj2 = {
    prop2: "obj2prop2",
    prop3: "obj2prop3"
};

var result = fjs.assign(obj1, obj2);
/* => {
    prop1: "obj1prop1",
    prop2: "obj1prop2",
    prop3: "obj2prop3"
} */
```

### Example extending arity

```js
var obj1 = {
    prop1: "obj1prop1",
    prop2: "obj1prop2"
};
var obj2 = {
    prop2: "obj2prop2",
    prop3: "obj2prop3",
    prop4: "obj2prop4"
};
var obj3 = {
    prop4: "obj3prop4",
    prop5: "obj3prop5"
};

var assignToObj1 = fjs.assign(obj1);
assignToObj1(obj2, obj3); // == fjs.assign(obj1, obj2, obj3);
/* => {
    prop1: "obj1prop1",
    prop2: "obj1prop2",
    prop3: "obj2prop3",
    prop4: "obj2prop4",
    prop5: "obj3prop5"
} */
```

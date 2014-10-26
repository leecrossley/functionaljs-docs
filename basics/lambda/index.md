title: Lambda expressions
description: Syntactically simple lambda expressions in functional.js
---

## Lambda expressions

fjs allows you to (optionally) specify lambda expressions, instead of bonafide JavaScript functions for any of it's curriable functions.

Multiple arguments can be separated by a comma and (an optional) space. The "goes to" lambda operator can be expressed as "=>" or "->".

### Curry example

```js
var concatenate = fjs.curry("a, b => a + b");

var concatenateHello = concatenate("Hello");

concatenateHello("World");
// => "HelloWorld"
```

The "concatenateHello" function is a higher order function created by partially invoking the "concatenate" function generated from the lambda expression with the first argument. "concatenateHello" can then be reused.

### Extend arity example

```js
var add = fjs.curry("a, b => a + b");

var add3 = add(3);

add(1, 2, 3) // => 6
add3(1, 2, 3, 4, 5) // => 18
```

### Map example

```js
var doubleMap = fjs.map("n => n * 2");

doubleMap([1, 2, 3]);
// => [2, 4, 6]
```

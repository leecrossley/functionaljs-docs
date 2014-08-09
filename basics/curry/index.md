title: Function currying with fjs.curry
description: Examples of currying JavaScript functions to create higher order functions for reuse.
---

## Currying

fjs.curry allows you to easily higher order functions by partially invoking an existing function, without supplying all the arguments of the original function.

### Basic example

```js
var concatenate = fjs.curry(function(word1, word2) {
    return word1 + " " + word2;
});

var concatenateHello = concatenate("Hello");

concatenateHello("World");
// => "Hello World"
```

The "concatenateHello" function is a higher order function created by partially invoking the "concatenate" function with the first argument. "concatenateHello" can then be reused.

### Another example

```js
var add = fjs.curry(function(arg1, arg2, arg3) {
    return arg1 + arg2 + arg3;
});

var add3 = add(3);
var add5 = add3(2);

add(3)(2)(1); // => 6
add3(2, 1); // => 6
add3(2)(1); // => 6
add5(1); // => 6
```

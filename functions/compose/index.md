title: Multiple function composition
description: λ.compose generates higher order functions by combining simpler functions.
---

## λ.compose

λ.compose facilitates *multiple function composition*. This is the generation of a higher order function by combining simpler functions.

### Usage

```js
λ.compose(functions);
```

### Example with 2 functions

```js
var f = function (a) {
    return "hello " + a;
};
var g = function (a) {
    return a + 1;
};
var composed = λ.compose(f, g);

composed(1); // => "hello 2"
```

The output from the right-most function is passed as the argument to the next function on the left, "hello 2" is then returned as a single result.

### Example with 3 functions

```js
var e = function (a) {
    return "hello " + a;
};
var f = function (a) {
    return a + 1;
};
var g = function (a) {
    return a * 100;
};
var composed = λ.compose(e, f, g);

composed(2); // => "hello 201"
```

This example illustrates the combining of multiple functions, passing the output from function "g" as a parameter to function "f", then passing the output from function "f" as a parameter to function "e". "hello 201" is then returned as a single result.

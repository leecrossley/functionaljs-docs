title: Extending arity with λ.curry
description: Examples of extending JavaScript function arity with λ.curry.
---

## Arity

The arity of a JavaScript function is the number of arguments *expected* by the function. With λ.curry it is possible to extend this arity beyond the expected length.

### Example

```js
var add = λ.curry(function(arg1, arg2) {
    return arg1 + arg2;
});

var add3 = add(3);

add(1, 2, 3); // => 6
add3(1, 2, 3, 4, 5); // => 18
```

The "add" function can now take any number of arguments (>= the expected arity) and the numbers will be summed. The "add" function can also be curried in the usual way by partial invocation (only supplying one argument, "add3").

The higher order function "add3" can also take any number of arguments, beyond the expected arity.

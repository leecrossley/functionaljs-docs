title: The functional JavaScript library
description: functional.js is a functional JavaScript library that facilitates currying and point-free / tacit programming.
---

[![Build Status](https://travis-ci.org/leecrossley/functional-js.png?branch=master)](https://travis-ci.org/leecrossley/functional-js) [![npm version](https://badge.fury.io/js/functional.js.png)](https://npmjs.org/package/functional.js) [![devDependency Status](https://david-dm.org/leecrossley/functional-js/dev-status.png)](https://david-dm.org/leecrossley/functional-js#info=devDependencies)

## What is functional.js?

functional.js is a functional JavaScript library. It facilitates [currying](http://en.wikipedia.org/wiki/Currying) and [point-free / tacit](http://en.wikipedia.org/wiki/Tacit_programming) programming and this methodology has been adhered to from the ground up.

## Is this like underscore.js?

Yes and no. There are many similar functions but libraries like underscore can't be curried in a regular fashion, as the items come before the iterator when supplied as arguments (e.g. (items, iterator) not (iterator, items)). There's also no support in underscore.js for functional-level programming, whereas this is the premise for functional.js.

functional.js is really lightweight and can be used instead of underscore.js. It also has no dependencies and doesn't extend any of JavaScript's standard built-in objects or use native functions that conditionalise implementations.

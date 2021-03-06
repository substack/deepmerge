deepmerge
=========

Merge the enumerable attributes of two objects deeply.

example
=======

``` js
var merge = require('deepmerge')
var x = { foo : { 'bar' : 3 } }
var y = { foo : { 'baz' : 4 }, quux : 5 }
var merged = merge(x, y)
console.dir(merged)
```

output:

```
{ foo: { bar: 3, baz: 4 }, quux: 5 }
```

methods
=======

var merge = require('deepmerge')

merge(x, y)
-----------

Merge two objects `x` and `y` deeply, returning a new merged object with the
elements from both `x` and `y`.

If an element at the same key is present for both `x` and `y`, the value from
`y` will appear in the result.

The merge is immutable, so neither `x` nor `y` will be modified.

install
=======

With [npm](http://npmjs.org) do:

```
npm install deepmerge
```

test
====

With [npm](http://npmjs.org) do:

```
npm test
```

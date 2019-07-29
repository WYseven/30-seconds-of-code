### flip

------------

Flip takes a function as an argument, then makes the first argument the last.

Return a closure that takes variadic inputs, and splices the last argument to make it the first argument before applying the rest.

------------

接受一个函数作为参数，然后将该函数第一个参数作为最后一个参数。（注：翻转参数）

返回一个接受可变参数输入的闭包，并且在应用其余参数之前将最后一个参数作为第一个参数。


```js
const flip = fn => (first, ...rest) => fn(...rest, first);
```

```js
let a = { name: 'John Smith' };
let b = {};
const mergeFrom = flip(Object.assign);
let mergePerson = mergeFrom.bind(null, a);
mergePerson(b); // == b
b = {};
Object.assign(b, a); // == b
```

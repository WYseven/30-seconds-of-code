### converge

------------

Accepts a converging function and a list of branching functions and returns a function that applies each branching function to the arguments and the results of the branching functions are passed as arguments to the converging function.

Use `Array.prototype.map()` and `Function.prototype.apply()` to apply each function to the given arguments.
Use the spread operator (`...`) to call `coverger` with the results of all other functions.

------------

接受聚合函数和分支函数列表，并返回一个函数，该函数将参数传递给每个分支函数，分支函数的结果作为参数传递给聚合函数。

使用 `Array.prototype.map()` 和 `function .prototype.apply()` 使每个函数处理给定的参数。
调用 `coverger` 使用 spread 操作符('...')得到所有其他函数的结果。

```js
const converge = (converger, fns) => (...args) => converger(...fns.map(fn => fn.apply(null, args)));
```

```js
const average = converge((a, b) => a / b, [
  arr => arr.reduce((a, v) => a + v, 0),
  arr => arr.length
]);
average([1, 2, 3, 4, 5, 6, 7]); // 4
```

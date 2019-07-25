### composeRight

Performs left-to-right function composition.

Use `Array.prototype.reduce()` to perform left-to-right function composition.
The first (leftmost) function can accept one or more arguments; the remaining functions must be unary.

执行从左到右的函数组合。

使用 `Array.prototype.reduce()` 执行从左到右的函数组合。
第一个(最左边的)函数可以接受一个或多个参数;其余的函数必须是接收一个参数的函数。

```js
const composeRight = (...fns) => fns.reduce((f, g) => (...args) => g(f(...args)));
```

```js
const add = (x, y) => x + y;
const square = x => x * x;
const addAndSquare = composeRight(add, square);
addAndSquare(1, 2); // 9
```

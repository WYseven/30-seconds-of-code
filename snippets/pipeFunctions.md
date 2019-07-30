### pipeFunctions

------------

Performs left-to-right function composition.

Use `Array.prototype.reduce()` with the spread operator (`...`) to perform left-to-right function composition.
The first (leftmost) function can accept one or more arguments; the remaining functions must be unary.

------------

从左到右执行函数组合。

使用 `Array.prototype.reduce()` 和扩展操作符 (`...`) 来执行从左到右的函数组合。
第一个(最左边)函数可以接受一个或多个参数;其余的函数只接受一个参数。

```js
const pipeFunctions = (...fns) => fns.reduce((f, g) => (...args) => g(f(...args)));
```

```js
const add5 = x => x + 5;
const multiply = (x, y) => x * y;
const multiplyAndAdd5 = pipeFunctions(multiply, add5);
multiplyAndAdd5(5, 2); // 15
```

### compose - 函数式编程术语：函数组合

Performs right-to-left function composition.

Use `Array.prototype.reduce()` to perform right-to-left function composition.
The last (rightmost) function can accept one or more arguments; the remaining functions must be unary.

执行从右到左的函数组合。

使用 `Array.prototype.reduce()` 执行从右到左的函数组合。
最后一个(最右边的)函数可以接受一个或多个参数;其余的函数必须是接收一个参数的函数。

```js
const compose = (...fns) => fns.reduce((f, g) => (...args) => f(g(...args)));
```

```js
const add5 = x => x + 5;
const multiply = (x, y) => x * y;
const multiplyAndAdd5 = compose(
  add5,
  multiply
);
multiplyAndAdd5(5, 2); // 15
```

### spreadOver

------------

Takes a variadic function and returns a closure that accepts an array of arguments to map to the inputs of the function.

Use closures and the spread operator (`...`) to map the array of arguments to the inputs of the function.

------------

接受一个可变参数的函数并返回一个闭包函数，该闭包函数接受要映射到函数的参数数组。

使用闭包和扩展操作符 (`...`) 将参数数组一一映射为函数的参数。

```js
const spreadOver = fn => argsArr => fn(...argsArr);
```

```js
const arrayMax = spreadOver(Math.max);
arrayMax([1, 2, 3]); // 3
```

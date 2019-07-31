### curry --- 函数式编程术语：柯里化

------------

Curries a function.

Use recursion.
If the number of provided arguments (`args`) is sufficient, call the passed function `fn`.
Otherwise, return a curried function `fn` that expects the rest of the arguments.
If you want to curry a function that accepts a variable number of arguments (a variadic function, e.g. `Math.min()`), you can optionally pass the number of arguments to the second parameter `arity`.

------------

柯里化一个函数。

使用递归。 
如果提供的参数 (`args`) 是函数 `fn` 接受的参数数量，则调用传递的函数 `fn`， 否则返回一个可接收剩余参数被柯里化后的函数 `fn`。
如果你想柯里化一个接受可变参数数量的函数(可变参数的函数，例如 `Math.min()` )，你可以选择将参数个数传递给第二个参数 `arity`。

```js
const curry = (fn, arity = fn.length, ...args) =>
  arity <= args.length ? fn(...args) : curry.bind(null, fn, arity, ...args);
```

```js
curry(Math.pow)(2)(10); // 1024
curry(Math.min, 3)(10)(50)(2); // 2
```

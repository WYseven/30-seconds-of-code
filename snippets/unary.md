### unary

------------

Creates a function that accepts up to one argument, ignoring any additional arguments.

Call the provided function, `fn`, with just the first argument given.

------------

创建一个函数，该函数最多只接受一个参数，忽略其他的参数。

调用提供的函数 `fn`，只需要给第一个参数即可。

```js
const unary = fn => val => fn(val);
```

```js
['6', '8', '10'].map(unary(parseInt)); // [6, 8, 10]
```

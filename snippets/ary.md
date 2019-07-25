### ary

Creates a function that accepts up to `n` arguments, ignoring any additional arguments.

Call the provided function, `fn`, with up to `n` arguments, using `Array.prototype.slice(0,n)` and the spread operator (`...`).


创建一个函数，该函数接受最多 `n` 个参数，忽略任何其他参数。

调用提供的函数 `fn`，参数最多为 `n`个，使用 `Array.prototype.slice(0,n)` 和 spread 操作符(`...`)提取并传入参数。


```js
const ary = (fn, n) => (...args) => fn(...args.slice(0, n));
```

```js
const firstTwoMax = ary(Math.max, 2);
[[2, 6, 'a'], [8, 4, 6], [10]].map(x => firstTwoMax(...x)); // [6, 8, 10]
```

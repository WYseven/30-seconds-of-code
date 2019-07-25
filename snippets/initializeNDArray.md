### initializeNDArray

------------

Create a n-dimensional array with given value.

Use recursion.
Use `Array.prototype.map()` to generate rows where each is a new array initialized using `initializeNDArray`.

------------

创建一个具有给定值的 `n` 维数组。

使用递归。
使用 `array.prototype.map()` 生成行，其中每个行都是使用 `initializeNDArray` 初始化的新数组。

```js
const initializeNDArray = (val, ...args) =>
  args.length === 0
    ? val
    : Array.from({ length: args[0] }).map(() => initializeNDArray(val, ...args.slice(1)));
```

```js
initializeNDArray(1, 3); // [1,1,1]
initializeNDArray(5, 2, 2, 2); // [[[5,5],[5,5]],[[5,5],[5,5]]]
```

### reduceSuccessive
【待翻译】
------------

Applies a function against an accumulator and each element in the array (from left to right), returning an array of successively reduced values.

Use `Array.prototype.reduce()` to apply the given function to the given array, storing each new result.

------------

对数组中的每个元素（从左到右）都应用累加器（accumulator）函数，返回依次减少一个值的数组。

使用 `array.prototype.reduce()` 将给定函数应用于给定数组，存储每个得到的新结果。

```js
const reduceSuccessive = (arr, fn, acc) =>
  arr.reduce((res, val, i, arr) => (res.push(fn(res.slice(-1)[0], val, i, arr)), res), [acc]);
```

```js
reduceSuccessive([1, 2, 3, 4, 5, 6], (acc, val) => acc + val, 0); // [0, 1, 3, 6, 10, 15, 21]
```


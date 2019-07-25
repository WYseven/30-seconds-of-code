### average

Returns the average of two or more numbers.

Use `Array.prototype.reduce()` to add each value to an accumulator, initialized with a value of `0`, divide by the `length` of the array.

返回两个或更多数字的平均值。

使用 `array. prototype.reduce()` 将每个值累加，初始值为 `0`，然后除以数组的 `length`。


```js
const average = (...nums) => nums.reduce((acc, val) => acc + val, 0) / nums.length;
```

```js
average(...[1, 2, 3]); // 2
average(1, 2, 3); // 2
```

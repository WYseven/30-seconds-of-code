### takeRight

------------

Returns an array with n elements removed from the end.

Use `Array.prototype.slice()` to create a slice of the array with `n` elements taken from the end.

------------

返回从结尾开始向前提取 `n` 个元素的数组。

使用 `array.prototype.slice()` 创建数组的一个切片，其中包含从结尾开始向前提取的 `n` 个元素。

```js
const takeRight = (arr, n = 1) => arr.slice(arr.length - n, arr.length);
```

```js
takeRight([1, 2, 3], 2); // [ 2, 3 ]
takeRight([1, 2, 3]); // [3]
```

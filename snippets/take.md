### take

------------

Returns an array with n elements removed from the beginning.

Use `Array.prototype.slice()` to create a slice of the array with `n` elements taken from the beginning.

------------

返回从开头开始提取 `n` 个元素的数组。

使用 `array.prototype.slice()` 创建数组的一个切片，其中包含从开头开始提取的 `n` 个元素。

```js
const take = (arr, n = 1) => arr.slice(0, n);
```

```js
take([1, 2, 3], 5); // [1, 2, 3]
take([1, 2, 3], 0); // []
```

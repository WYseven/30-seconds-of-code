### chunk

Chunks an array into smaller arrays of a specified size.

Use `Array.from()` to create a new array, that fits the number of chunks that will be produced.
Use `Array.prototype.slice()` to map each element of the new array to a chunk the length of `size`.
If the original array can't be split evenly, the final chunk will contain the remaining elements.

将数组分块成指定大小的较小数组。

使用 `array.from()` 创建一个新的数组，该数组的长度就是将要生成的块（chunk）的个数。
使用 `array.prototype.slice()` 将新数组的每个元素映射为一个长度为 `size` 的块（chunk）。
如果原始数组不能被平均分割，那么最后的块（chunk）将包含剩余的元素。

```js
const chunk = (arr, size) =>
  Array.from({ length: Math.ceil(arr.length / size) }, (v, i) =>
    arr.slice(i * size, i * size + size)
  );
```

```js
chunk([1, 2, 3, 4, 5], 2); // [[1,2],[3,4],[5]]
```

### dropRight

------------

Returns a new array with `n` elements removed from the right.

Use `Array.prototype.slice()` to remove the specified number of elements from the right.

------------

返回从右侧开始删除 `n` 个元素的新数组。

使用 `Array.prototype.slice()` 从右侧删除指定数量的元素。

```js
const dropRight = (arr, n = 1) => arr.slice(0, -n);
```

```js
dropRight([1, 2, 3]); // [1,2]
dropRight([1, 2, 3], 2); // [1]
dropRight([1, 2, 3], 42); // []
```

### drop

Returns a new array with `n` elements removed from the left.

Use `Array.prototype.slice()` to remove the specified number of elements from the left.

返回从左侧开始删除 `n` 个元素的新数组。

使用 `Array.prototype.slice()` 从左边删除指定数量的元素。

```js
const drop = (arr, n = 1) => arr.slice(n);
```

```js
drop([1, 2, 3]); // [2,3]
drop([1, 2, 3], 2); // [3]
drop([1, 2, 3], 42); // []
```

### indexOfAll

------------

Returns all indices of `val` in an array.
If `val` never occurs, returns `[]`.

Use `Array.prototype.reduce()` to loop over elements and store indices for matching elements.
Return the array of indices.

------------

返回数组中 `val` 的所有索引。如果在数组中没找到 `val`，则返回 `[]` 。

使用 `Array.prototype.reduce()` 循环元素并存储匹配元素的索引。
返回索引数组。

```js
const indexOfAll = (arr, val) => arr.reduce((acc, el, i) => (el === val ? [...acc, i] : acc), []);
```

```js
indexOfAll([1, 2, 3, 1, 2, 3], 1); // [0,3]
indexOfAll([1, 2, 3], 4); // []
```

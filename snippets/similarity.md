### similarity

------------

Returns an array of elements that appear in both arrays.

Use `Array.prototype.filter()` to remove values that are not part of `values`, determined using `Array.prototype.includes()`.

------------

返回两个数组的交集。

使用 `Array.prototype.filter()` 移除不属于 `values` 中的值，这些值由 `array .prototype.include()` 来确定。

```js
const similarity = (arr, values) => arr.filter(v => values.includes(v));
```

```js
similarity([1, 2, 3], [1, 2, 4]); // [1, 2]
```

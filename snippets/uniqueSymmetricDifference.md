### uniqueSymmetricDifference

------------

Returns the unique symmetric difference between two arrays, not containing duplicate values from either array.

Use `Array.prototype.filter()` and `Array.prototype.includes()` on each array to remove values contained in the other, then create a `Set` from the results, removing duplicate values.

------------

返回两个数组的差集，在两个数组中不重复的值。

在每个数组上使用 `array.prototype.filter()` 和 `array .prototype.include()` 来过滤另一个数组中包含的值，然后从结果中创建一个 `Set` ，删除重复的值。

```js
const uniqueSymmetricDifference = (a, b) => [
  ...new Set([...a.filter(v => !b.includes(v)), ...b.filter(v => !a.includes(v))])
];
```

```js
uniqueSymmetricDifference([1, 2, 3], [1, 2, 4]); // [3, 4]
uniqueSymmetricDifference([1, 2, 2], [1, 3, 1]); // [2, 3]
```

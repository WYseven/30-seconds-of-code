### symmetricDifference

------------

Returns the symmetric difference between two arrays, without filtering out duplicate values.

Create a `Set` from each array, then use `Array.prototype.filter()` on each of them to only keep values not contained in the other.

------------

返回两个数组之间的差集，而不过滤重复的值。

根据每个数组创建一个 `Set` ，然后在每个数组上使用 `array.prototype.filter()` ，只保留不包含在另一个数组中的值。

```js
const symmetricDifference = (a, b) => {
  const sA = new Set(a),
    sB = new Set(b);
  return [...a.filter(x => !sB.has(x)), ...b.filter(x => !sA.has(x))];
};
```

```js
symmetricDifference([1, 2, 3], [1, 2, 4]); // [3, 4]
symmetricDifference([1, 2, 2], [1, 3, 1]); // [2, 2, 3]
```

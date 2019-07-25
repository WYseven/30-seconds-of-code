### symmetricDifferenceBy

------------

Returns the symmetric difference between two arrays, after applying the provided function to each array element of both.

Create a `Set` by applying `fn` to each array's elements, then use `Array.prototype.filter()` on each of them to only keep values not contained in the other.

------------

将提供的函数应用于两个数组的每个元素后，返回两个数组之间的差集。

根据每个数组创建一个 `Set` ，然后在每个数组上使用 `array.prototype.filter()` ，只保留不包含在另一个数组中的值。

```js
const symmetricDifferenceBy = (a, b, fn) => {
  const sA = new Set(a.map(v => fn(v))),
    sB = new Set(b.map(v => fn(v)));
  return [...a.filter(x => !sB.has(fn(x))), ...b.filter(x => !sA.has(fn(x)))];
};
```

```js
symmetricDifferenceBy([2.1, 1.2], [2.3, 3.4], Math.floor); // [ 1.2, 3.4 ]
```

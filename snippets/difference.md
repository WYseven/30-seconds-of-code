### difference

Returns the difference between two arrays.

Create a `Set` from `b`, then use `Array.prototype.filter()` on `a` to only keep values not contained in `b`.

返回两个数组之间的差异。

根据数组 `b` 创建一个 `Set` 对象，然后在数组 `a` 上使用 `Array.filter()` 方法，过滤出数组 `b` 中不包含的值。

```js
const difference = (a, b) => {
  const s = new Set(b);
  return a.filter(x => !s.has(x));
};
```

```js
difference([1, 2, 3], [1, 2, 4]); // [3]
```

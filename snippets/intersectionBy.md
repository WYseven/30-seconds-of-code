### intersectionBy

------------

Returns a list of elements that exist in both arrays, after applying the provided function to each array element of both.

Create a `Set` by applying `fn` to all elements in `b`, then use `Array.prototype.filter()` on `a` to only keep elements, which produce values contained in `b` when `fn` is applied to them.

------------

将提供的函数应用于两个数组的每个数组元素后，返回两个数组中存在的元素列表。

将 `fn` 应用于 `b` 中的所有元素来创建 `Set` 对象 ，然后在 `a` 上使用 `Array.prototype.filter()`，只保留调用 `fn` 应用于每个元素后，同时在 `b` 中存在的元素。

```js
const intersectionBy = (a, b, fn) => {
  const s = new Set(b.map(fn));
  return a.filter(x => s.has(fn(x)));
};
```

```js
intersectionBy([2.1, 1.2], [2.3, 3.4], Math.floor); // [2.1]
```

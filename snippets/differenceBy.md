### differenceBy

------------

Returns the difference between two arrays, after applying the provided function to each array element of both.

Create a `Set` by applying `fn` to each element in `b`, then use `Array.prototype.map()` to apply `fn` to each element in `a`, then `Array.prototype.filter()`

------------

将提供的函数应用于两个数组的每个数组元素后，返回两个数组之间的差值。

将 `fn` 处理数组 `b` 中的每个元素后创建 `Set`，然后使用 `Array.prototype.map（）` 映射 `fn` 处理数组 `a` 中的每个元素，最后应用`Array.prototype.filter（）` 进行过滤。

```js
const differenceBy = (a, b, fn) => {
  const s = new Set(b.map(fn));
  return a.map(fn).filter(el => !s.has(el));
};
```

```js
differenceBy([2.1, 1.2], [2.3, 3.4], Math.floor); // [1]
differenceBy([{ x: 2 }, { x: 1 }], [{ x: 1 }], v => v.x); // [2]
```

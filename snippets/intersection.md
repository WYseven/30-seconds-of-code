### intersection

------------

Returns a list of elements that exist in both arrays.

Create a `Set` from `b`, then use `Array.prototype.filter()` on `a` to only keep values contained in `b`.

------------

返回两个数组中都存在的元素列表。

根据数组 `b` 创建一个 `Set` 对象，然后在数组 `a` 上使用 `Array.prototype.filter()` 方法，只保留数组 `b` 中也包含的值。

```js
const intersection = (a, b) => {
  const s = new Set(b);
  return a.filter(x => s.has(x));
};
```

```js
intersection([1, 2, 3], [4, 3, 2]); // [2, 3]
```

### unionWith

------------

Returns every element that exists in any of the two arrays once, using a provided comparator function.

Create a `Set` with all values of `a` and values in `b` for which the comparator finds no matches in `a`, using `Array.prototype.findIndex()`.

------------

使用提供的比较器函数，返回两个数组的并集，相同的元素只出现一次。

用 `Array.prototype.findIndex()` 使用提供的比较器函数后，在 `b` 中查找没有在 `a` 中匹配的值。

```js
const unionWith = (a, b, comp) =>
  Array.from(new Set([...a, ...b.filter(x => a.findIndex(y => comp(x, y)) === -1)]));
```

```js
unionWith([1, 1.2, 1.5, 3, 0], [1.9, 3, 0, 3.9], (a, b) => Math.round(a) === Math.round(b)); // [1, 1.2, 1.5, 3, 0, 3.9]
```

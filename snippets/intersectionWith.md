### intersectionWith

------------

Returns a list of elements that exist in both arrays, using a provided comparator function.

Use `Array.prototype.filter()` and `Array.prototype.findIndex()` in combination with the provided comparator to determine intersecting values.

------------

使用提供的比较器（comparator）函数，返回两个数组中存在的元素列表。

使用 `Array.prototype.filter()` 和 `Array.prototype.findIndex()` 结合比较器（comparator）函数来确定交叉值。

```js
const intersectionWith = (a, b, comp) => a.filter(x => b.findIndex(y => comp(x, y)) !== -1);
```

```js
intersectionWith([1, 1.2, 1.5, 3, 0], [1.9, 3, 0, 3.9], (a, b) => Math.round(a) === Math.round(b)); // [1.5, 3, 0]
```

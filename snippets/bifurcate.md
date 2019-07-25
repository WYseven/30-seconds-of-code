### bifurcate

------------

Splits values into two groups. If an element in `filter` is truthy, the corresponding element in the collection belongs to the first group; otherwise, it belongs to the second group.

Use `Array.prototype.reduce()` and `Array.prototype.push()` to add elements to groups, based on `filter`.

------------

将值分成两组，如果 `filter` 中的元素为 `true`，则集合中对应的元素属于第一组;否则，它属于第二组。

基于 `filter`，使用 `Array.prototype.reduce()` 和 `Array.prototype.push()` 向组添加元素。

```js
const bifurcate = (arr, filter) =>
  arr.reduce((acc, val, i) => (acc[filter[i] ? 0 : 1].push(val), acc), [[], []]);
```

```js
bifurcate(['beep', 'boop', 'foo', 'bar'], [true, true, false, true]); // [ ['beep', 'boop', 'bar'], ['foo'] ]
```

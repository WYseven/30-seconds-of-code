### filterNonUniqueBy

Filters out the non-unique values in an array, based on a provided comparator function.

Use `Array.prototype.filter()` and `Array.prototype.every()` for an array containing only the unique values, based on the comparator function, `fn`.
The comparator function takes four arguments: the values of the two elements being compared and their indexes.

根据提供的比较器（comparator）函数，过滤数组中的非唯一值。

基于比较器函数 `fn` ，使用 `array .prototype.filter()` 和 `array .prototype.every()` 对数组过滤后，数组中只包含唯一值。

比较器函数接受四个参数:正在比较的两个元素的值及其索引。

```js
const filterNonUniqueBy = (arr, fn) =>
  arr.filter((v, i) => arr.every((x, j) => (i === j) === fn(v, x, i, j)));
```

```js
filterNonUniqueBy(
  [
    { id: 0, value: 'a' },
    { id: 1, value: 'b' },
    { id: 2, value: 'c' },
    { id: 1, value: 'd' },
    { id: 0, value: 'e' }
  ],
  (a, b) => a.id == b.id
); // [ { id: 2, value: 'c' } ]
```

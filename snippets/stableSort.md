### stableSort

------------

Performs stable sorting of an array, preserving the initial indexes of items when their values are the same.
Does not mutate the original array, but returns a new array instead.

Use `Array.prototype.map()` to pair each element of the input array with its corresponding index.
Use `Array.prototype.sort()` and a `compare` function to sort the list, preserving their initial order if the items compared are equal.
Use `Array.prototype.map()` to convert back to the initial array items.

------------

对数组执行稳定排序，值相同时保留其初始索引。
不改变原始数组，而是返回新数组。

使用 `array.prototype.map()` 将输入数组的每个元素与其对应的索引配对。
使用 `Array.prototype.sort()` 和 `compare` 函数对列表进行排序，如果比较的值相等，则保留它们的初始顺序。
使用 `array.prototype.map()` 将其转换回初始数组项。

```js
const stableSort = (arr, compare) =>
  arr
    .map((item, index) => ({ item, index }))
    .sort((a, b) => compare(a.item, b.item) || a.index - b.index)
    .map(({ item }) => item);
```

```js
const arr = [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
const stable = stableSort(arr, () => 0); // [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
```

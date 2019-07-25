### sortedIndexBy

------------

Returns the lowest index at which value should be inserted into array in order to maintain its sort order, based on a provided iterator function.

Check if the array is sorted in descending order (loosely).
Use `Array.prototype.findIndex()` to find the appropriate index where the element should be inserted, based on the iterator function `fn`.

------------

返回根据提供的迭代器函数，将指定值插入到数组中的最小索引位置，以保持其排序顺序。

检查数组是否按降序(松散地)排序。
使用 `Array.prototype.findIndex()` 根据迭代器函数 `fn` 查找应该插入元素的适当索引。

```js
const sortedIndexBy = (arr, n, fn) => {
  const isDescending = fn(arr[0]) > fn(arr[arr.length - 1]);
  const val = fn(n);
  const index = arr.findIndex(el => (isDescending ? val >= fn(el) : val <= fn(el)));
  return index === -1 ? arr.length : index;
};
```

```js
sortedIndexBy([{ x: 4 }, { x: 5 }], { x: 4 }, o => o.x); // 0
```

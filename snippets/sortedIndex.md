### sortedIndex

------------

Returns the lowest index at which value should be inserted into array in order to maintain its sort order.

Check if the array is sorted in descending order (loosely).
Use `Array.prototype.findIndex()` to find the appropriate index where the element should be inserted.

------------

返回指定值插入到数组中的最小索引位置，以保持其排序顺序。

检查数组是否按降序（松散地）排序。 使用 `Array.prototype.findIndex()` 找到元素应该被插入的合适的索引位置。


```js
const sortedIndex = (arr, n) => {
  const isDescending = arr[0] > arr[arr.length - 1];
  const index = arr.findIndex(el => (isDescending ? n >= el : n <= el));
  return index === -1 ? arr.length : index;
};
```

```js
sortedIndex([5, 3, 2, 1], 4); // 1
sortedIndex([30, 50], 40); // 1
```

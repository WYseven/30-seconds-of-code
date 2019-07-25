### sortedLastIndex

------------

Returns the highest index at which value should be inserted into array in order to maintain its sort order.

Check if the array is sorted in descending order (loosely).
Use `Array.prototype.reverse()` and `Array.prototype.findIndex()` to find the appropriate last index where the element should be inserted.

------------

返回指定值插入到数组中的最大索引位置，以保持其排序顺序。

检查数组是否按降序(松散地)排序。
使用 `Array.prototype.reverse()` 和 ` Array.prototype.findIndex()` 查找应该插入元素的最后一个适当的索引。

```js
const sortedLastIndex = (arr, n) => {
  const isDescending = arr[0] > arr[arr.length - 1];
  const index = arr.reverse().findIndex(el => (isDescending ? n <= el : n >= el));
  return index === -1 ? 0 : arr.length - index;
};
```

```js
sortedLastIndex([10, 20, 30, 30, 40], 30); // 4
```

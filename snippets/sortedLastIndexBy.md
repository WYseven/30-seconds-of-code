### sortedLastIndexBy

------------

Returns the highest index at which value should be inserted into array in order to maintain its sort order, based on a provided iterator function.

Check if the array is sorted in descending order (loosely).
Use `Array.prototype.map()` to apply the iterator function to all elements of the array.
Use `Array.prototype.reverse()` and `Array.prototype.findIndex()` to find the appropriate last index where the element should be inserted, based on the provided iterator function.

------------

返回根据提供的迭代器函数，将指定值插入到数组中的最大索引位置，以保持其排序顺序。

检查数组是否按降序(松散地)排序。
使用 `array.prototype.map()` 将迭代器函数应用于数组的所有元素。
使用 `Array.prototype.reverse()` 和 ` Array.prototype.findIndex()` 根据提供的迭代器函数，查找应该插入元素的最后一个适当的索引。


```js
const sortedLastIndexBy = (arr, n, fn) => {
  const isDescending = fn(arr[0]) > fn(arr[arr.length - 1]);
  const val = fn(n);
  const index = arr
    .map(fn)
    .reverse()
    .findIndex(el => (isDescending ? val <= el : val >= el));
  return index === -1 ? 0 : arr.length - index;
};
```

```js
sortedLastIndexBy([{ x: 4 }, { x: 5 }], { x: 4 }, o => o.x); // 1
```

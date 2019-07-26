### dropRightWhile

------------

Removes elements from the end of an array until the passed function returns `true`. Returns the remaining elements in the array.

Loop through the array, using `Array.prototype.slice()` to drop the last element of the array until the returned value from the function is `true`.
Returns the remaining elements.

------------

从数组末尾移除元素，直到传递的函数返回 `true` 。返回数组中剩余的元素。

从数组的末尾开始循环遍历数组，使用 `array.prototype.slice()` 删除数组中第一个遇到函数返回的值为 `true` 位置的元素。
返回数组中剩余的元素。

```js
const dropRightWhile = (arr, func) => {
  let rightIndex = arr.length;
  while (rightIndex-- && !func(arr[rightIndex]));
  return arr.slice(0, rightIndex + 1);
};
```

```js
dropRightWhile([1, 2, 3, 4], n => n < 3); // [1, 2]
```

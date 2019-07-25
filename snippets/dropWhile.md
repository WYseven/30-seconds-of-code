### dropWhile

Removes elements in an array until the passed function returns `true`. Returns the remaining elements in the array.

Loop through the array, using `Array.prototype.slice()` to drop the first element of the array until the returned value from the function is `true`.
Returns the remaining elements.

移除数组中的元素，直到传递的函数返回 `true` 。 返回数组中剩余的元素。

循环遍历数组，使用 `array.prototype.slice()` 删除数组中第一个遇到函数返回的值为 `true` 位置的元素。
返回数组中剩余的元素。

```js
const dropWhile = (arr, func) => {
  while (arr.length > 0 && !func(arr[0])) arr = arr.slice(1);
  return arr;
};
```

```js
dropWhile([1, 2, 3, 4], n => n >= 3); // [3,4]
```

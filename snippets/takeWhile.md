### takeWhile

------------

Removes elements in an array until the passed function returns `true`. Returns the removed elements.

Loop through the array, using a `for...of` loop over `Array.prototype.entries()` until the returned value from the function is `true`.
Return the removed elements, using `Array.prototype.slice()`.

------------

从数组的开头开始删除数组中的元素，直到传递的函数返回 `true` 。返回删除的元素。

循环遍历数组，使用 `for...of` 循环 `Array.prototype.entries()` 拿到的值， 直到函数返回的值为 `true` 为止。
使用 `Array.prototype.slice()` 返回删除的元素。

```js
const takeWhile = (arr, func) => {
  for (const [i, val] of arr.entries()) if (func(val)) return arr.slice(0, i);
  return arr;
};
```

```js
takeWhile([1, 2, 3, 4], n => n >= 3); // [1, 2]
```

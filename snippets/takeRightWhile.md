### takeRightWhile

------------

Removes elements from the end of an array until the passed function returns `true`. Returns the removed elements.

Loop through the array, using a `Array.prototype.reduceRight()` and accumulating elements while the function returns falsy value.

------------

从数组末尾移除元素，直到传递的函数返回“true”。返回删除的元素。

```js
const takeRightWhile = (arr, func) =>
  arr.reduceRight((acc, el) => (func(el) ? acc : [el, ...acc]), []);
```

```js
takeRightWhile([1, 2, 3, 4], n => n < 3); // [3, 4]
```

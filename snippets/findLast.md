### findLast

Returns the last element for which the provided function returns a truthy value.

Use `Array.prototype.filter()` to remove elements for which `fn` returns falsy values, `Array.prototype.pop()` to get the last one.

通过提供的函数返回值为真值（truthy）过滤数组，返回这个数组最后一个元素。

使用 `Array.prototype.filter()` 过滤掉 `fn` 返回假值（falsy）的元素， 用 `Array.prototype.pop()` 获取最后一个值。

```js
const findLast = (arr, fn) => arr.filter(fn).pop();
```

```js
findLast([1, 2, 3, 4], n => n % 2 === 1); // 3
```

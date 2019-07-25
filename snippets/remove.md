### remove

------------

Removes elements from an array for which the given function returns `false`.

Use `Array.prototype.filter()` to find array elements that return truthy values and `Array.prototype.reduce()` to remove elements using `Array.prototype.splice()`.
The `func` is invoked with three arguments (`value, index, array`).

------------

从数组中移除给定函数返回 `false` 的元素。

使用 `Array.prototype.filter()`  和 `Array.prototype.reduce()` 来查找数组中返回真值的元素，使用 `Array.prototype.splice()` 来移除元素。 `func` 有三个参数 (`value, index, array`)。

```js
const remove = (arr, func) =>
  Array.isArray(arr)
    ? arr.filter(func).reduce((acc, val) => {
      arr.splice(arr.indexOf(val), 1);
      return acc.concat(val);
    }, [])
    : [];
```

```js
remove([1, 2, 3, 4], n => n % 2 === 0); // [2, 4]
```

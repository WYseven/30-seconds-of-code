### uniqueElements

------------

Returns all unique values of an array.

Use ES6 `Set` and the `...rest` operator to discard all duplicated values.

------------

返回去重后的数组。

使用 ES6 的 `Set` 和 `...rest` 运算符去除所有重复的值。

```js
const uniqueElements = arr => [...new Set(arr)];
```

```js
uniqueElements([1, 2, 2, 3, 4, 4, 5]); // [1, 2, 3, 4, 5]
```

### maxN

------------

Returns the `n` maximum elements from the provided array.
If `n` is greater than or equal to the provided array's length, then return the original array (sorted in descending order).

Use `Array.prototype.sort()` combined with the spread operator (`...`) to create a shallow clone of the array and sort it in descending order.
Use `Array.prototype.slice()` to get the specified number of elements.
Omit the second argument, `n`, to get a one-element array.

------------

从提供的数组中返回 `n` 个最大值元素。
如果 `n` 大于或等于提供的数组长度，则返回原始数组(按降序排列)。

使用 `array.prototype.sort()` 和 展开操作符 (`...`) 对数组进行浅克隆，并按降序排序。
使用 `Array.prototype.slice()` 获取指定数量的元素。
省略第二个参数 `n` ，获得只有一个元素的数组。

```js
const maxN = (arr, n = 1) => [...arr].sort((a, b) => b - a).slice(0, n);
```

```js
maxN([1, 2, 3]); // [3]
maxN([1, 2, 3], 2); // [3,2]
```

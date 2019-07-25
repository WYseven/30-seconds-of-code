### countOccurrences

Counts the occurrences of a value in an array.

Use `Array.prototype.reduce()` to increment a counter each time you encounter the specific value inside the array.

计算数组中值的出现次数。

每次在数组中遇到指定的值时，使用 `array. prototype.reduce()` 递增计数器。

```js
const countOccurrences = (arr, val) => arr.reduce((a, v) => (v === val ? a + 1 : a), 0);
```

```js
countOccurrences([1, 1, 2, 1, 2, 3], 1); // 3
```

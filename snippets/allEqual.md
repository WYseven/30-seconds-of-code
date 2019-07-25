### allEqual

------------

Check if all elements in an array are equal.

Use `Array.prototype.every()` to check if all the elements of the array are the same as the first one.
Elements in the array are compared using the strict comparison operator, which does not account for `NaN` self-inequality.

------------

检查数组中的所有元素是否相等。

使用 `Array.prototype.every()` 检查数组中的所有元素是否与第一个元素相同。
使用严格比较运算符比较数组中的元素，该运算符不考虑 `NaN` 与自己不相等的情况。

```js
const allEqual = arr => arr.every(val => val === arr[0]);
```

```js
allEqual([1, 2, 3, 4, 5, 6]); // false
allEqual([1, 1, 1, 1]); // true
```

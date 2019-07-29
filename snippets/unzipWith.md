### unzipWith

------------

Creates an array of elements, ungrouping the elements in an array produced by [zip](#zip) and applying the provided function.

Use `Math.max.apply()` to get the longest subarray in the array, `Array.prototype.map()` to make each element an array.
Use `Array.prototype.reduce()` and `Array.prototype.forEach()` to map grouped values to individual arrays.
Use `Array.prototype.map()` and the spread operator (`...`) to apply `fn` to each individual group of elements.

------------

创建一个数组，将 [zip](#zip) 生成的数组中的元素取消分组，并结合提供的函数生成最后的结果。

使用 `Math.max.apply()` 获取数组中最长子数组的长度，使用 `Array.prototype.map()` 生成最长长度个数组。
使用 `Array.prototype.reduce()` 和 `Array.prototype.forEach()` 将分组元素映射到对应的数组中。
使用 `Array.prototype.map()` 和展开操作符 (`...`) 将 `fn` 应用于每一组元素。

```js
const unzipWith = (arr, fn) =>
  arr
    .reduce(
      (acc, val) => (val.forEach((v, i) => acc[i].push(v)), acc),
      Array.from({
        length: Math.max(...arr.map(x => x.length))
      }).map(x => [])
    )
    .map(val => fn(...val));
```

```js
unzipWith([[1, 10, 100], [2, 20, 200]], (...args) => args.reduce((acc, v) => acc + v, 0)); // [3, 30, 300]
```

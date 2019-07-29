### unzip

------------

Creates an array of arrays, ungrouping the elements in an array produced by [zip](#zip).

Use `Math.max.apply()` to get the longest subarray in the array, `Array.prototype.map()` to make each element an array.
Use `Array.prototype.reduce()` and `Array.prototype.forEach()` to map grouped values to individual arrays.

------------

创建一个数组，将 [zip](#zip) 生成的数组中的元素取消分组。

使用 `Math.max.apply()` 获取数组中最长子数组的长度，使用 `Array.prototype.map()` 生成最长长度个数组。
使用 `Array.prototype.reduce()` 和 `Array.prototype.forEach()` 将分组元素映射到对应的数组中。


```js
const unzip = arr =>
  arr.reduce(
    (acc, val) => (val.forEach((v, i) => acc[i].push(v)), acc),
    Array.from({
      length: Math.max(...arr.map(x => x.length))
    }).map(x => [])
  );
```

```js
unzip([['a', 1, true], ['b', 2, false]]); // [['a', 'b'], [1, 2], [true, false]]
unzip([['a', 1, true], ['b', 2]]); // [['a', 'b'], [1, 2], [true]]
```

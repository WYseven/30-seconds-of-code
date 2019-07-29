### xProd

------------

Creates a new array out of the two supplied by creating each possible pair from the arrays.

Use `Array.prototype.reduce()`, `Array.prototype.map()` and `Array.prototype.concat()` to produce every possible pair from the elements of the two arrays and save them in an array.

------------

将两个数组的每个元素两两进行组合，组合出所有的可能对存在数组中，返回一个存在所有可能性对的数组。

使用 `Array.prototype.reduce()`, `Array.prototype.map()` 和 `Array.prototype.concat()` 从两个数组的元素中生成所有可能的对，并将它们保存在一个数组中。

```js
const xProd = (a, b) => a.reduce((acc, x) => acc.concat(b.map(y => [x, y])), []);
```

```js
xProd([1, 2], ['a', 'b']); // [[1, 'a'], [1, 'b'], [2, 'a'], [2, 'b']]
```

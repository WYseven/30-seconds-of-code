### deepFlatten

------------

Deep flattens an array.

Use recursion.
Use `Array.prototype.concat()` with an empty array (`[]`) and the spread operator (`...`) to flatten an array.
Recursively flatten each element that is an array.

------------

深度平铺一个数组。

使用递归。
使用 `array. prototype.concat()` 和空数组( `[]` )，结合 spread 操作符('...')将数组平铺。
递归平铺数组中的每个元素。

```js
const deepFlatten = arr => [].concat(...arr.map(v => (Array.isArray(v) ? deepFlatten(v) : v)));
```

```js
deepFlatten([1, [2], [[3], 4], 5]); // [1,2,3,4,5]
```

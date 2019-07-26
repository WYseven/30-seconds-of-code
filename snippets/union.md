### union

------------

Returns every element that exists in any of the two arrays once.

Create a `Set` with all values of `a` and `b` and convert to an array.

------------

返回两个数组的并集，相同的元素只出现一次。

基于 `a` 和 `b` 创建一个 `Set` 对象，返回转换后的数组。

```js
const union = (a, b) => Array.from(new Set([...a, ...b]));
```

```js
union([1, 2, 3], [4, 3, 2]); // [1,2,3,4]
```

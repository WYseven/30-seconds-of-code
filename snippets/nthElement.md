### nthElement

------------

Returns the nth element of an array.

Use `Array.prototype.slice()` to get an array containing the nth element at the first place.
If the index is out of bounds, return `undefined`.
Omit the second argument, `n`, to get the first element of the array.

------------

返回数组的第 `n` 个元素。

使用 `array .prototype.slice()` 首先获得一个包含第 n 个元素的数组。
如果索引超出界限，返回 `undefined` 。
省略第二个参数 `n` ，获得数组的第一个元素。

```js
const nthElement = (arr, n = 0) => (n === -1 ? arr.slice(n) : arr.slice(n, n + 1))[0];
```

```js
nthElement(['a', 'b', 'c'], 1); // 'b'
nthElement(['a', 'b', 'b'], -3); // 'a'
```

### without

------------

Filters out the elements of an array, that have one of the specified values.

Use `Array.prototype.filter()` to create an array excluding(using `!Array.includes()`) all given values.

_(For a snippet that mutates the original array see [`pull`](#pull))_

------------

过滤掉数组中具有指定值之一的元素。

使用 `array.prototype.filter()` 创建一个数组，排除(使用 `!array.include()` )所有给定值。

_(改变原始数组，请看 [`pull`](#pull)) 代码片段_

```js
const without = (arr, ...args) => arr.filter(v => !args.includes(v));
```

```js
without([2, 1, 2, 3], 1, 2); // [3]
```

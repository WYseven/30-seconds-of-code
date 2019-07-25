### sample

------------

Returns a random element from an array.

Use `Math.random()` to generate a random number, multiply it by `length` and round it off to the nearest whole number using `Math.floor()`.
This method also works with strings.

------------

从数组中返回一个随机元素。

使用 `Math.random()` 生成随机数，将其乘以 `length` ，并使用 `Math.floor()` 将其四舍五入到最近的整数。
这个方法也适用于字符串。


```js
const sample = arr => arr[Math.floor(Math.random() * arr.length)];
```

```js
sample([3, 7, 9, 11]); // 9
```

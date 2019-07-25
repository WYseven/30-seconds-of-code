### approximatelyEqual

Checks if two numbers are approximately equal to each other.

Use `Math.abs()` to compare the absolute difference of the two values to `epsilon`.
Omit the third parameter, `epsilon`, to use a default value of `0.001`.

检查两个数是否近似相等。

使用 `Math.abs()` 将两个值的绝对差值与 `epsilon` 进行比较。
省略第三个参数 `epsilon`，使用默认值`0.001`。


```js
const approximatelyEqual = (v1, v2, epsilon = 0.001) => Math.abs(v1 - v2) < epsilon;
```

```js
approximatelyEqual(Math.PI / 2.0, 1.5708); // true
```

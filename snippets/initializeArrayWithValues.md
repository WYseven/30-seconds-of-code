### initializeArrayWithValues

------------

Initializes and fills an array with the specified values.

Use `Array(n)` to create an array of the desired length, `fill(v)` to fill it with the desired values.
You can omit `val` to use a default value of `0`.

------------

使用指定的值初始化和填充数组。

使用 `Array(n)` 创建所需长度的数组，使用 `fill(v)` 填充所需的值。 你可以忽略 `val` ，使用默认值 `0`。


```js
const initializeArrayWithValues = (n, val = 0) => Array(n).fill(val);
```

```js
initializeArrayWithValues(5, 2); // [2, 2, 2, 2, 2]
```

### initialize2DArray

------------

Initializes a 2D array of given width and height and value.

Use `Array.prototype.map()` to generate h rows where each is a new array of size w initialize with value. If the value is not provided, default to `null`.

------------

初始化一个给定行数和列数，以及值的二维数组。

使用 `array.prototype.map()` 生成 `h` 行，其中每一行都是长度为 `w` 的新数组。如果没有提供值 `val`，则默认为 `null`。


```js
const initialize2DArray = (w, h, val = null) =>
  Array.from({ length: h }).map(() => Array.from({ length: w }).fill(val));
```

```js
initialize2DArray(2, 2, 0); // [[0,0], [0,0]]
```

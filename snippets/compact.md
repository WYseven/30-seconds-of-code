### compact

------------

Removes falsy values from an array.

Use `Array.prototype.filter()` to filter out falsy values (`false`, `null`, `0`, `""`, `undefined`, and `NaN`).

------------

从数组中删除为 `false` 的值。

使用 `Array.prototype.filter()` 过滤掉数组中所有为假值的元素 (`false`, `null`, `0`, `""`, `undefined`, 和 `NaN`)。

```js
const compact = arr => arr.filter(Boolean);
```

```js
compact([0, 1, false, 2, '', 3, 'a', 'e' * 23, NaN, 's', 34]); // [ 1, 2, 3, 'a', 's', 34 ]
```

### filterFalsy

Filters out the falsy values in an array.

Use `Array.prototype.filter()` to get an array containing only truthy values.

过滤数组中为假值（falsy）的元素。

使用 `array .prototype.filter()` 过滤后，数组中只包含为真值（truthy）的元素。

```js
const filterFalsy = arr => arr.filter(Boolean);
```

```js
filterFalsy(['', true, {}, false, 'sample', 1, 0]); // [true, {}, 'sample', 1]
```

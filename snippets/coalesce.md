### coalesce

Returns the first non-null/undefined argument.

Use `Array.prototype.find()` to return the first non `null`/`undefined` argument.

返回第一个不是 `null` 或 `undefined` 的参数。

使用 `Array.prototype.find()` 返回第一个不是 `null` 或 `undefined` 的参数。

```js
const coalesce = (...args) => args.find(_ => ![undefined, null].includes(_));
```

```js
coalesce(null, undefined, '', NaN, 'Waldo'); // ""
```

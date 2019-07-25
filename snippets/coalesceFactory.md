### coalesceFactory

Returns a customized coalesce function that returns the first argument that returns `true` from the provided argument validation function.

Use `Array.prototype.find()` to return the first argument that returns `true` from the provided argument validation function.

返回一个自定义的 `coalesce` 函数，该函数返回从提供的参数验证函数返回为 `true` 的第一个参数。

使用 `Array.prototype.find()` 返回从提供的参数验证函数返回 `true` 的第一个参数。
```js
const coalesceFactory = valid => (...args) => args.find(valid);
```

```js
const customCoalesce = coalesceFactory(_ => ![null, undefined, '', NaN].includes(_));
customCoalesce(undefined, null, NaN, '', 'Waldo'); // "Waldo"
```

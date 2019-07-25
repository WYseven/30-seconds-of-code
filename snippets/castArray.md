### castArray

Casts the provided value as an array if it's not one.

Use `Array.prototype.isArray()` to determine if `val` is an array and return it as-is or encapsulated in an array accordingly.

如果提供的值不是数组，则将其转换为数组。

使用 `array.prototype.isarray()` 来确定 `val` 是否是一个数组，如果是数组，按原样返回；如果不是数组，将值封装在数组中返回。

```js
const castArray = val => (Array.isArray(val) ? val : [val]);
```

```js
castArray('foo'); // ['foo']
castArray([1]); // [1]
```

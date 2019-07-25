### any

------------

Returns `true` if the provided predicate function returns `true` for at least one element in a collection, `false` otherwise.

Use `Array.prototype.some()` to test if any elements in the collection return `true` based on `fn`.
Omit the second argument, `fn`, to use `Boolean` as a default.

------------

如果提供的断言函数（predicate function）对集合中所有的元素测试，至少有一个返回 `true`，那么 `any` 方法就返回 `true`。否则，返回 `false`。

使用 `Array.prototype.some()` 测试集合中的所有元素是否基于 `fn` 返回 `true`。
省略第二个参数`fn`，使用 `Boolean` 作为默认值。

```js
const any = (arr, fn = Boolean) => arr.some(fn);
```

```js
any([0, 1, 2, 0], x => x >= 2); // true
any([0, 0, 1, 0]); // true
```

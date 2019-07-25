### all

------------

Returns `true` if the provided predicate function returns `true` for all elements in a collection, `false` otherwise.

Use `Array.prototype.every()` to test if all elements in the collection return `true` based on `fn`.
Omit the second argument, `fn`, to use `Boolean` as a default.

------------

如果提供的断言函数（predicate function）对集合中所有的元素测试都返回 `true`，那么 `all` 方法就返回 `true`。否则，返回 `false`。

使用 `Array.prototype.every()` 测试集合中的所有元素是否基于 `fn` 返回 `true`。
省略第二个参数`fn`，使用 `Boolean` 作为默认值。

```js
const all = (arr, fn = Boolean) => arr.every(fn);
```

```js
all([4, 2, 3], x => x > 1); // true
all([1, 2, 3]); // true
```

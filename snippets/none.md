### none

------------

Returns `true` if the provided predicate function returns `false` for all elements in a collection, `false` otherwise.

Use `Array.prototype.some()` to test if any elements in the collection return `true` based on `fn`.
Omit the second argument, `fn`, to use `Boolean` as a default.

------------

如果提供的断言（predicate）函数处理集合中的所有元素都返回 `false` ，则返回 `true` ，否则返回 `false` 。

使用 `Array.prototype.some()` 测试集合中的任何元素是否基于 `fn` 返回 `true` 。
省略第二个参数 `fn` ，使用 `Boolean` 作为默认值。

```js
const none = (arr, fn = Boolean) => !arr.some(fn);
```

```js
none([0, 1, 3, 0], x => x == 2); // true
none([0, 0, 0]); // true
```

### flatten

Flattens an array up to the specified depth.

Use recursion, decrementing `depth` by 1 for each level of depth.
Use `Array.prototype.reduce()` and `Array.prototype.concat()` to merge elements or arrays.
Base case, for `depth` equal to `1` stops recursion.
Omit the second argument, `depth` to flatten only to a depth of `1` (single flatten).

将数组展平到指定的深度。

使用递归，为每个深度级别 `depth` 递减 `1`。 使用 `Array.prototype.reduce()` 和 `Array.prototype.concat()` 来合并元素或数组。 基本情况下，`depth` 等于 `1` 停止递归。 省略第二个参数，`depth` 只能平铺到 `1` 层(单层平铺) 的深度。

```js
const flatten = (arr, depth = 1) =>
  arr.reduce((a, v) => a.concat(depth > 1 && Array.isArray(v) ? flatten(v, depth - 1) : v), []);
```

```js
flatten([1, [2], 3, 4]); // [1, 2, 3, 4]
flatten([1, [2, [3, [4, 5], 6], 7], 8], 2); // [1, 2, 3, [4, 5], 6, 7, 8]
```

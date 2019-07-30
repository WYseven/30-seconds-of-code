### rearg

------------

Creates a function that invokes the provided function with its arguments arranged according to the specified indexes.

Use `Array.prototype.map()` to reorder arguments based on `indexes` in combination with the spread operator (`...`) to pass the transformed arguments to `fn`.

------------

创建一个函数，该函数调用提供的函数，并根据指定的索引排列参数。

使用 `Array.prototype.map()` 根据 `indexes` 和扩展操作符 (`...`) 对参数重新排序，将转换后的参数传递给 `fn` 。

```js
const rearg = (fn, indexes) => (...args) => fn(...indexes.map(i => args[i]));
```

```js
var rearged = rearg(
  function(a, b, c) {
    return [a, b, c];
  },
  [2, 0, 1]
);
rearged('b', 'c', 'a'); // ['a', 'b', 'c']
```

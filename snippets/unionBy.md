### unionBy

------------

Returns every element that exists in any of the two arrays once, after applying the provided function to each array element of both.

Create a `Set` by applying all `fn` to all values of `a`.
Create a `Set` from `a` and all elements in `b` whose value, after applying `fn` does not match a value in the previously created set.
Return the last set converted to an array.

------------

将所提供的函数应用于两个数组的每个元素之后，返回两个数组的并集，相同的元素只出现一次。

在 `fn` 应用于 `a` 的所有元素后创建一个 `Set`，并在 `b` 中过滤已经在集合中存在的元素。
最后返回一个转换为数组的集合。

```js
const unionBy = (a, b, fn) => {
  const s = new Set(a.map(fn));
  return Array.from(new Set([...a, ...b.filter(x => !s.has(fn(x)))]));
};
```

```js
unionBy([2.1], [1.2, 2.3], Math.floor); // [2.1, 1.2]
```

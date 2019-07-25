### partition

------------

Groups the elements into two arrays, depending on the provided function's truthiness for each element.

Use `Array.prototype.reduce()` to create an array of two arrays.
Use `Array.prototype.push()` to add elements for which `fn` returns `true` to the first array and elements for which `fn` returns `false` to the second one.

------------

根据提供的函数对每个元素进行迭代，将元素分组为两个数组。

使用 `array.prototype.reduce()` 创建一个由两个数组组成的数组。
使用 `array.prototype.push()` 将 `fn` 返回 `true` 的元素添加到第一个数组，而 `fn` 返回 `false` 的元素添加到第二个数组。

```js
const partition = (arr, fn) =>
  arr.reduce(
    (acc, val, i, arr) => {
      acc[fn(val, i, arr) ? 0 : 1].push(val);
      return acc;
    },
    [[], []]
  );
```

```js
const users = [{ user: 'barney', age: 36, active: false }, { user: 'fred', age: 40, active: true }];
partition(users, o => o.active); // [[{ 'user': 'fred',    'age': 40, 'active': true }],[{ 'user': 'barney',  'age': 36, 'active': false }]]
```

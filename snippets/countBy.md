### countBy

Groups the elements of an array based on the given function and returns the count of elements in each group.

Use `Array.prototype.map()` to map the values of an array to a function or property name.
Use `Array.prototype.reduce()` to create an object, where the keys are produced from the mapped results.

根据给定函数对数组的元素进行分组，并返回每个组中的元素数量。

使用 `array .prototype.map()` 将数组的值映射到函数或属性名称。
使用 `Array.prototype.reduce()` 创建一个对象，其中键（`key`）是从映射的结果中产生的。

```js
const countBy = (arr, fn) =>
  arr.map(typeof fn === 'function' ? fn : val => val[fn]).reduce((acc, val) => {
    acc[val] = (acc[val] || 0) + 1;
    return acc;
  }, {});
```

```js
countBy([6.1, 4.2, 6.3], Math.floor); // {4: 1, 6: 2}
countBy(['one', 'two', 'three'], 'length'); // {3: 2, 5: 1}
```

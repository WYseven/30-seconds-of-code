### groupBy

Groups the elements of an array based on the given function.

Use `Array.prototype.map()` to map the values of an array to a function or property name.
Use `Array.prototype.reduce()` to create an object, where the keys are produced from the mapped results.

根据给定的函数对数组的元素进行分组。

使用 `Array.prototype.map()` 将数组的值映射到函数或属性名称。使用 `Array.prototype.reduce()` 来创建一个对象，其中的 `key` 是从映射结果中产生。

```js
const groupBy = (arr, fn) =>
  arr.map(typeof fn === 'function' ? fn : val => val[fn]).reduce((acc, val, i) => {
    acc[val] = (acc[val] || []).concat(arr[i]);
    return acc;
  }, {});
```

```js
groupBy([6.1, 4.2, 6.3], Math.floor); // {4: [4.2], 6: [6.1, 6.3]}
groupBy(['one', 'two', 'three'], 'length'); // {3: ['one', 'two'], 5: ['three']}
```

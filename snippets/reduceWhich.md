### reduceWhich

------------

Returns the minimum/maximum value of an array, after applying the provided function to set comparing rule.

Use `Array.prototype.reduce()` in combination with the `comparator` function to get the appropriate element in the array.
You can omit the second parameter, `comparator`, to use the default one that returns the minimum element in the array.

------------

将提供的函数设置比较规则后应用于数组，返回数组的最小/最大值。

使用 `array.prototype.reduce()` 结合 `comparator` 函数来获取数组中合适的元素。
您可以省略第二个参数 `comparator` ，默认返回数组中最小的元素。

```js
const reduceWhich = (arr, comparator = (a, b) => a - b) =>
  arr.reduce((a, b) => (comparator(a, b) >= 0 ? b : a));
```

```js
reduceWhich([1, 3, 2]); // 1
reduceWhich([1, 3, 2], (a, b) => b - a); // 3
reduceWhich(
  [{ name: 'Tom', age: 12 }, { name: 'Jack', age: 18 }, { name: 'Lucy', age: 9 }],
  (a, b) => a.age - b.age
); // {name: "Lucy", age: 9}
```

### reducedFilter

------------

Filter an array of objects based on a condition while also filtering out unspecified keys.

Use `Array.prototype.filter()` to filter the array based on the predicate `fn` so that it returns the objects for which the condition returned a truthy value.
On the filtered array, use `Array.prototype.map()` to return the new object using `Array.prototype.reduce()` to filter out the keys which were not supplied as the `keys` argument.

------------

根据条件过滤一个对象数组，同时过滤掉未指定的键。

使用 `array.prototype.filter()` 根据断言函数 `fn` 对数组进行过滤，返回条件为真值（truthy）的对象。
在经过过滤后的数组上，使用 `array.prototype.map()` 和 `array.prototype.reduce()` 过滤掉在 `keys` 参数中未提供的键。

```js
const reducedFilter = (data, keys, fn) =>
  data.filter(fn).map(el =>
    keys.reduce((acc, key) => {
      acc[key] = el[key];
      return acc;
    }, {})
  );
```

```js
const data = [
  {
    id: 1,
    name: 'john',
    age: 24
  },
  {
    id: 2,
    name: 'mike',
    age: 50
  }
];

reducedFilter(data, ['id', 'name'], item => item.age > 24); // [{ id: 2, name: 'mike'}]
```

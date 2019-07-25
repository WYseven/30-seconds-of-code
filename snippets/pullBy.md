### pullBy

------------

Mutates the original array to filter out the values specified, based on a given iterator function.

Check if the last argument provided in a function.
Use `Array.prototype.map()` to apply the iterator function `fn` to all array elements.
Use `Array.prototype.filter()` and `Array.prototype.includes()` to pull out the values that are not needed.
Use `Array.prototype.length = 0` to mutate the passed in an array by resetting it's length to zero and `Array.prototype.push()` to re-populate it with only the pulled values.

------------


根据给定的迭代器（iterator）函数，修改原始数组，过滤掉指定的值。

检查函数中是否提供了最后一个参数。
使用 `array.prototype.map()` 将迭代器函数 `fn` 应用于所有数组元素。
使用 `Array.prototype.filter()` 和 `array.prototype.include()` 过滤指定的值。
使用 `Array.prototype.length = 0` 通过将数组的长度重置为0来清空数组，并使用 `array.prototype.push()` 把提取的值重新填充数组。

```js
const pullBy = (arr, ...args) => {
  const length = args.length;
  let fn = length > 1 ? args[length - 1] : undefined;
  fn = typeof fn == 'function' ? (args.pop(), fn) : undefined;
  let argState = (Array.isArray(args[0]) ? args[0] : args).map(val => fn(val));
  let pulled = arr.filter((v, i) => !argState.includes(fn(v)));
  arr.length = 0;
  pulled.forEach(v => arr.push(v));
};
```

```js
var myArray = [{ x: 1 }, { x: 2 }, { x: 3 }, { x: 1 }];
pullBy(myArray, [{ x: 1 }, { x: 3 }], o => o.x); // myArray = [{ x: 2 }]
```

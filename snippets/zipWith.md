### zipWith

------------

Creates an array of elements, grouped based on the position in the original arrays and using function as the last value to specify how grouped values should be combined.

Check if the last argument provided is a function.
Use `Math.max()` to get the longest array in the arguments.
Creates an array with that length as return value and use `Array.from()` with a map-function to create an array of grouped elements.
If lengths of the argument-arrays vary, `undefined` is used where no value could be found.
The function is invoked with the elements of each group `(...group)`.

------------

创建一个根据原始数组中的位置进行分组的数组，并使用函数作为最后一个参数来指定应如何组合分组中的值。

检查最后提供的参数是否为函数。
使用 `Math.max.apply()` 获取参数中最长的数组，创建一个长度为该长度的数组，并使用`Array.from()`  和映射函数（map-function） 来创建一个分组元素数组。 
如果参数数组的长度不同，则在找不到值的地方使用“undefined”。
最后一个参数提供的函数应用于每个组 `(...group)` 的元素。


```js
const zipWith = (...array) => {
  const fn = typeof array[array.length - 1] === 'function' ? array.pop() : undefined;
  return Array.from(
    { length: Math.max(...array.map(a => a.length)) },
    (_, i) => (fn ? fn(...array.map(a => a[i])) : array.map(a => a[i]))
  );
};
```

```js
zipWith([1, 2], [10, 20], [100, 200], (a, b, c) => a + b + c); // [111,222]
zipWith(
  [1, 2, 3],
  [10, 20],
  [100, 200],
  (a, b, c) => (a != null ? a : 'a') + (b != null ? b : 'b') + (c != null ? c : 'c')
); // [111, 222, '3bc']
```

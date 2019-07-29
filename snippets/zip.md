### zip

------------

Creates an array of elements, grouped based on the position in the original arrays.

Use `Math.max.apply()` to get the longest array in the arguments.
Creates an array with that length as return value and use `Array.from()` with a map-function to create an array of grouped elements.
If lengths of the argument-arrays vary, `undefined` is used where no value could be found.

------------

创建一个根据原始数组中的位置进行分组的数组。

使用 `Math.max.apply()` 获取参数中最长的数组，创建一个长度为该长度的数组，并使用`Array.from()`  和映射函数（map-function） 来创建一个分组元素数组。 如果参数数组的长度不同，则在未找到值的情况下使用 `undefined` 。

```js
const zip = (...arrays) => {
  const maxLength = Math.max(...arrays.map(x => x.length));
  return Array.from({ length: maxLength }).map((_, i) => {
    return Array.from({ length: arrays.length }, (_, k) => arrays[k][i]);
  });
};
```

```js
zip(['a', 'b'], [1, 2], [true, false]); // [['a', 1, true], ['b', 2, false]]
zip(['a'], [1, 2], [true, false]); // [['a', 1, true], [undefined, 2, false]]
```

### pullAtIndex

------------

Mutates the original array to filter out the values at the specified indexes.

  Use `Array.prototype.filter()` and `Array.prototype.includes()` to pull out the values that are not needed.
  Use `Array.prototype.length = 0` to mutate the passed in an array by resetting it's length to zero and `Array.prototype.push()` to re-populate it with only the pulled values.
  Use `Array.prototype.push()` to keep track of pulled values

------------

改变原始数组，过滤掉指定索引的值。

使用 `Array.prototype.filter()` 和 `array.prototype.include()` 过滤指定的值。
使用 `Array.prototype.length = 0` 通过将数组的长度重置为0来清空数组，并使用 `array.prototype.push()` 把提取的值重新填充数组。
使用 `Array.prototype.push()` 跟踪提取的值。


```js
const pullAtIndex = (arr, pullArr) => {
  let removed = [];
  let pulled = arr
    .map((v, i) => (pullArr.includes(i) ? removed.push(v) : v))
    .filter((v, i) => !pullArr.includes(i));
  arr.length = 0;
  pulled.forEach(v => arr.push(v));
  return removed;
};
```

```js
let myArray = ['a', 'b', 'c', 'd'];
let pulled = pullAtIndex(myArray, [1, 3]); // myArray = [ 'a', 'c' ] , pulled = [ 'b', 'd' ]
```

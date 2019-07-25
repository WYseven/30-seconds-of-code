### pull

------------

Mutates the original array to filter out the values specified.

Use `Array.prototype.filter()` and `Array.prototype.includes()` to pull out the values that are not needed.
Use `Array.prototype.length = 0` to mutate the passed in an array by resetting it's length to zero and `Array.prototype.push()` to re-populate it with only the pulled values.

_(For a snippet that does not mutate the original array see [`without`](#without))_

------------

改变原始数组，过滤掉指定的值。

使用 `Array.prototype.filter()` 和 `array.prototype.include()` 过滤指定的值。
使用 `Array.prototype.length = 0` 通过将数组的长度重置为0来清空数组，并使用 `array.prototype.push()` 把提取的值重新填充数组。

_(对于不改变原始数组的代码片段，请参阅 [`without`](#without))_

```js
const pull = (arr, ...args) => {
  let argState = Array.isArray(args[0]) ? args[0] : args;
  let pulled = arr.filter((v, i) => !argState.includes(v));
  arr.length = 0;
  pulled.forEach(v => arr.push(v));
};
```

```js
let myArray = ['a', 'b', 'c', 'a', 'b', 'c'];
pull(myArray, 'a', 'c'); // myArray = [ 'b', 'b' ]
```

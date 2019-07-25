### shank

------------

Has the same functionality as [`Array.prototype.splice()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/splice), but returning a new array instead of mutating the original array.

Use `Array.prototype.slice()` and `Array.prototype.concat()` to get a new array with the new contents after removing existing elements and/or adding new elements.
Omit the second argument, `index`, to start at `0`.
Omit the third argument, `delCount`, to remove `0` elements.
Omit the fourth argument, `elements`, in order to not add any new elements.

------------

具有与[`Array.prototype.splice()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/splice)相同的功能，但是 `Array.prototype.splice()` 返回一个新数组，而不是修改原始数组。

在删除现有元素 和/或 添加新元素之后，使用 `array.prototype.slice()` 和 `array.prototype.concat()` 获得一个包含新内容的新数组。
省略第二个参数 `index` ，下标从 `0` 开始。
省略第三个参数 `delCount` ，删除 `0` 个元素。
省略第四个参数 `elements` ，不添加任何新元素。

```js
const shank = (arr, index = 0, delCount = 0, ...elements) =>
  arr
    .slice(0, index)
    .concat(elements)
    .concat(arr.slice(index + delCount));
```

```js
const names = ['alpha', 'bravo', 'charlie'];
const namesAndDelta = shank(names, 1, 0, 'delta'); // [ 'alpha', 'delta', 'bravo', 'charlie' ]
const namesNoBravo = shank(names, 1, 1); // [ 'alpha', 'charlie' ]
console.log(names); // ['alpha', 'bravo', 'charlie']
```

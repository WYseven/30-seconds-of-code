### offset

------------

Moves the specified amount of elements to the end of the array.

Use `Array.prototype.slice()` twice to get the elements after the specified index and the elements before that.
Use the spread operator(`...`) to combine the two into one array.
If `offset` is negative, the elements will be moved from end to start.

------------

将指定数量的元素移动到数组的末尾。

两次使用 `Array.prototype.slice()` 来获取指定索引之后的元素和指定索引之前的元素。
使用展开操作符(`...`)将两个数组合成一个数组。
如果 `offset` 为负数，元素将从结束移动到开始位置。

```js
const offset = (arr, offset) => [...arr.slice(offset), ...arr.slice(0, offset)];
```

```js
offset([1, 2, 3, 4, 5], 2); // [3, 4, 5, 1, 2]
offset([1, 2, 3, 4, 5], -2); // [4, 5, 1, 2, 3]
```

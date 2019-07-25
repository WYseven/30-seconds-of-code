### initializeArrayWithRangeRight
[待翻译]
------------

Initializes an array containing the numbers in the specified range (in reverse) where `start` and `end` are inclusive with their common difference `step`.

Use `Array.from(Math.ceil((end+1-start)/step))` to create an array of the desired length(the amounts of elements is equal to `(end-start)/step` or `(end+1-start)/step` for inclusive end), `Array.prototype.map()` to fill with the desired values in a range.
You can omit `start` to use a default value of `0`.
You can omit `step` to use a default value of `1`.

------------

初始化一个数组，该数组包含指定范围 `start` 到 `end` 内的数字（反向），可设置间隔 `step`。

使用 `array.from(Math.ceil((end+1-start)/step)` 来创建所需长度的数组(元素的数量等于 `(end-start)/step` 或 `(end+1-start)/step` ，包含结束数字)， 使用 `array.prototype.map()` 来填充范围中所需要的值。

```js
const initializeArrayWithRangeRight = (end, start = 0, step = 1) =>
  Array.from({ length: Math.ceil((end + 1 - start) / step) }).map(
    (v, i, arr) => (arr.length - i - 1) * step + start
  );
```

```js
initializeArrayWithRangeRight(5); // [5,4,3,2,1,0]
initializeArrayWithRangeRight(7, 3); // [7,6,5,4,3]
initializeArrayWithRangeRight(9, 0, 2); // [8,6,4,2,0]
```

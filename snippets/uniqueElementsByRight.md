### uniqueElementsByRight

------------

Returns all unique values of an array, based on a provided comparator function, starting from the right.

Use `Array.prototype.reduceRight()` and `Array.prototype.some()` for an array containing only the last unique occurrence of each value, based on the comparator function, `fn`.
The comparator function takes two arguments: the values of the two elements being compared.

------------

根据提供的比较器函数，从右边开始，返回去重后的数组。

根据比较器函数 `fn`， 从右边开始，使用 `Array.prototype.reduceRight()` 和 `Array.prototype.some()` 去除重复的值，只保留重复值中最后一个出现的值。
比较器（comparator）函数接受两个参数：正在比较的两个元素的值。

```js
const uniqueElementsByRight = (arr, fn) =>
  arr.reduceRight((acc, v) => {
    if (!acc.some(x => fn(v, x))) acc.push(v);
    return acc;
  }, []);
```

```js
uniqueElementsByRight(
  [
    { id: 0, value: 'a' },
    { id: 1, value: 'b' },
    { id: 2, value: 'c' },
    { id: 1, value: 'd' },
    { id: 0, value: 'e' }
  ],
  (a, b) => a.id == b.id
); // [ { id: 0, value: 'e' }, { id: 1, value: 'd' }, { id: 2, value: 'c' } ]
```

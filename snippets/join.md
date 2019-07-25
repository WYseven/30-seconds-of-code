### join

------------

Joins all elements of an array into a string and returns this string.
Uses a separator and an end separator.

Use `Array.prototype.reduce()` to combine elements into a string.
Omit the second argument, `separator`, to use a default separator of `','`.
Omit the third argument, `end`, to use the same value as `separator` by default.

------------

将数组的所有元素拼接成一个字符串并返回此字符串。 使用分隔符和结束分隔符。

使用 `Array.prototype.reduce()` 将元素拼接成一个字符串。 省略第二个参数 `separator` ，则默认使用分隔符','。 省略第三个参数 `end` ，默认使用与 `separator` 相同的值。

```js
const join = (arr, separator = ',', end = separator) =>
  arr.reduce(
    (acc, val, i) =>
      i === arr.length - 2
        ? acc + val + end
        : i === arr.length - 1
          ? acc + val
          : acc + val + separator,
    ''
  );
```

```js
join(['pen', 'pineapple', 'apple', 'pen'], ',', '&'); // "pen,pineapple,apple&pen"
join(['pen', 'pineapple', 'apple', 'pen'], ','); // "pen,pineapple,apple,pen"
join(['pen', 'pineapple', 'apple', 'pen']); // "pen,pineapple,apple,pen"
```

### capitalize

Capitalizes the first letter of a string.

Use array destructuring and `String.prototype.toUpperCase()` to capitalize first letter, `...rest` to get array of characters after first letter and then `Array.prototype.join('')` to make it a string again.
Omit the `lowerRest` parameter to keep the rest of the string intact, or set it to `true` to convert to lowercase.


将字符串的第一个字母大写。

使用数组解构和 `String.prototype.toUpperCase()` 把第一个字母大写，`...rest ` 获取第一个字母后的字符组成的数组，然后 `array .prototype.join(")` 将其再次变为字符串。
省略 `lowerRest` 参数保持字符串的其余部分不变，或将其设置为 `true` 将字符串的剩余部分都转换为小写。

```js
const capitalize = ([first, ...rest], lowerRest = false) =>
  first.toUpperCase() + (lowerRest ? rest.join('').toLowerCase() : rest.join(''));
```

```js
capitalize('fooBar'); // 'FooBar'
capitalize('fooBar', true); // 'Foobar'
```

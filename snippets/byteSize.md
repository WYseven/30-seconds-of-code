### byteSize

Returns the length of a string in bytes.

Convert a given string to a [`Blob` Object](https://developer.mozilla.org/en-US/docs/Web/API/Blob) and find its `size`.

以字节为单位返回字符串的长度。

将给定的字符串转换为[`Blob Object`]（https://developer.mozilla.org/en-US/docs/Web/API/Blob）并找到它的`size`。

```js
const byteSize = str => new Blob([str]).size;
```

```js
byteSize('😀'); // 4
byteSize('Hello World'); // 11
```

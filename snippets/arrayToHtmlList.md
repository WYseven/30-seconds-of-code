### arrayToHtmlList

------------

Converts the given array elements into `<li>` tags and appends them to the list of the given id.

Use `Array.prototype.map()`, `document.querySelector()`, and an anonymous inner closure to create a list of html tags.

------------

将给定的数组元素转换为 `<li>` 标签，并将它们添加到给定 id 的列表中。

使用 `Array.prototype.map()` 、`document.querySelector()` 和内部闭包创建 `html` 标签列表。

```js
const arrayToHtmlList = (arr, listID) =>
  (el => (
    (el = document.querySelector('#' + listID)),
    (el.innerHTML += arr.map(item => `<li>${item}</li>`).join(''))
  ))();
```

```js
arrayToHtmlList(['item 1', 'item 2'], 'myListID');
```

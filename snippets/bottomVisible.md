### bottomVisible

------------

Returns `true` if the bottom of the page is visible, `false` otherwise.

Use `scrollY`, `scrollHeight` and `clientHeight` to determine if the bottom of the page is visible.

------------

如果页面底部可见，返回 `true`，否则返回 `false`。
使用 `scrollY`, `scrollHeight` 和 `clientHeight` 来判断页面的底部是否可见。

```js
const bottomVisible = () =>
  document.documentElement.clientHeight + window.scrollY >=
  (document.documentElement.scrollHeight || document.documentElement.clientHeight);
```

```js
bottomVisible(); // true
```

### bind

------------

Creates a function that invokes `fn` with a given context, optionally adding any additional supplied parameters to the beginning of the arguments.

Return a `function` that uses `Function.prototype.apply()` to apply the given `context` to `fn`.
Use `Array.prototype.concat()` to prepend any additional supplied parameters to the arguments.

------------

创建一个函数，该函数使用给定的上下文调用 `fn`，最初的参数列表中添加任何额外提供的可选参数。

返回一个 `function`，它使用 `Function.prototype.apply()` 将给定的 `context` 应用于 `fn`。
使用 spread 操作符(`...`) 将任何额外提供的可选参数添加到参数列表中，并传递给 `fn`。

```js
const bind = (fn, context, ...boundArgs) => (...args) => fn.apply(context, [...boundArgs, ...args]);
```

```js
function greet(greeting, punctuation) {
  return greeting + ' ' + this.user + punctuation;
}
const freddy = { user: 'fred' };
const freddyBound = bind(greet, freddy);
console.log(freddyBound('hi', '!')); // 'hi fred!'
```

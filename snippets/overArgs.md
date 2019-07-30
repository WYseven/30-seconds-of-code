### overArgs

------------

Creates a function that invokes the provided function with its arguments transformed.

Use `Array.prototype.map()` to apply `transforms` to `args` in combination with the spread operator (`...`) to pass the transformed arguments to `fn`.

------------

创建一个函数，该函数调用所提供的函数并对传入的参数进行转换。

使用 `Array.prototype.map()` 将 `transform` 应用于 `args` ，并结合扩展操作符 (`...`) 将转换后的参数传递给 `fn` 。

```js
const overArgs = (fn, transforms) => (...args) => fn(...args.map((val, i) => transforms[i](val)));
```

```js
const square = n => n * n;
const double = n => n * 2;
const fn = overArgs((x, y) => [x, y], [square, double]);
fn(9, 3); // [81, 6]
```

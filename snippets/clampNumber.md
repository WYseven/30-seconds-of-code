### clampNumber

Clamps `num` within the inclusive range specified by the boundary values `a` and `b`.

If `num` falls within the range, return `num`.
Otherwise, return the nearest number in the range.

将num夹在由边值a和b指定的包含范围内。

在边界值“a”和“b”指定的包含范围内钳位`num`。

返回由边界值 `a` 和 `b` 限定范围内的 `num` 。

如果 `num` 在限定范围内，则返回 `num`。 否则，返回范围内最接近 `num` 的数字。

```js
const clampNumber = (num, a, b) => Math.max(Math.min(num, Math.max(a, b)), Math.min(a, b));
```

```js
clampNumber(2, 3, 5); // 3
clampNumber(1, -1, -5); // -1
```

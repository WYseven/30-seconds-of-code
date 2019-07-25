### checkProp

Given a `predicate` function and a `prop` string, this curried function will then take an `object` to inspect by calling the property and passing it to the predicate.

Summon `prop` on `obj`, pass it to a provided `predicate` function and return a masked boolean.

待翻译。。。。。。

给定一个 `predicate` 断言函数和一个 `prop` 字符串，这个柯里化（curried）函数将通过调用该属性并将其传递给断言来接收一个 `object` 进行检查。

这个柯里化（curried）函数将接收一个 `object`，把对象访问的属性，传递给断言函数，


```js
const checkProp = (predicate, prop) => obj => !!predicate(obj[prop]);
```

```js


const lengthIs4 = checkProp(l => l === 4, 'length');
lengthIs4([]); // false
lengthIs4([1,2,3,4]); // true
lengthIs4(new Set([1,2,3,4])); // false (Set uses Size, not length)

const session = { user: {} };
const validUserSession = checkProps(u => u.active && !u.disabled, 'user');

validUserSession(session); // false

session.user.active = true;
validUserSession(session); // true

const noLength(l => l === undefined, 'length');
noLength([]); // false
noLength({}); // true
noLength(new Set()); // true
```

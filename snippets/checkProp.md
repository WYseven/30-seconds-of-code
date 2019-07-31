### checkProp

------------

Given a `predicate` function and a `prop` string, this curried function will then take an `object` to inspect by calling the property and passing it to the predicate.

Summon `prop` on `obj`, pass it to a provided `predicate` function and return a masked boolean.

------------

给定一个断言（predicate）函数和一个 `prop` 字符串，这个柯里化（curried）函数将接收一个 `object` 对象，把对象访问的属性值，传递给断言函数，

调用 `obj` 上的 `prop` ，将它传递给提供的 `predicate` 函数，并返回一个布尔值。

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

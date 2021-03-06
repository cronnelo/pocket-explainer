# Block scoping

`let` and `const` are said to be "block scoping." In JavaScript, a block is code inside *{ ... }*. These variables are only available inside their blocks.

```js
if (true) {
  let a = 'hello'
}
console.log(a)  //=> undefined
```

> ↳ `a` is only available inside the *if* block.

There are more blocks than `if`s:

```js
function greet () { /*...*/ }
if (hidden) { /*...*/ }
else { /*...*/ }
try { /*...*/ }
catch (e) { /*...*/ }
finally { /*...*/ }
switch (state) { /*...*/ }
for (;;) { /*...*/ }
while (true) { /*...*/ }
```

-

> What about blocks inside blocks? [Continue >](nested-blocks.md)

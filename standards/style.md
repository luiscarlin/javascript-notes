# Crockford Style

- use JSLint for code quality
- use:
```js
right {
}
```
- good style reduces errors
- no space when calling a funciton -> `myFun(bar);`
- one space if not calling a function ->

  - `return (foo);`
  - `if (a == b)`
  - `function (x) { ... }`

- self invoking functions:
```js
(function () {
  ...
}());
```
- never rely on automatic semicolon insertion. Always add yours.
- do not use `with` statement
- confusion must be avoided
- always use `===` never `==`
- multi-line string literals is error prone (an extra space will break it)
- JS only has function scope (no block scope)
- `var` declarations get hoisted to the top of the functin (because valid in the scope), but the initialization remains where it was
  (moral: in function scope languages, always declare & initialize vars at top of your function)
- functions are hoisted as well, so declare them all at the top as well
- `for (var i = 0; ... ; ... )` <= var i's scope is not the loop, but everywhere inside that function
- Global vars are evil, avoid them. If you need to use them, use UPPER_CASE
- constructor functions should be named with InitialCaps (and nothing else should). Only in these scenarios you can use `new`
- never use `var = a = b = 0` because leads to confusion.
- **KEY: Write in a way that clearly communicates your intent**
- `"let"` doesn't do hoisting of variables. **Always use it.**
- no need to pack things in one line.
- instead of `x++` use `x += 1`
- always use braces for if statements (even if one line after if)
- **styles that can hide defects are considered defective**
- JS is a deeply flawed language

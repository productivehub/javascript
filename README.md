# ProductiveHub JavaScript Style Guide() {

ProductiveHub official JavaScript (and TypeScript ) styleguide.

## Table of Contents

1. [Naming Conventions](#references)
1. [Comments](#comments)



## Naming Conventions

Reference eslint: [id-length](https://eslint.org/docs/rules/id-length)

Avoid very short or very long identifier names. Be descriptive with your naming

```javascript
// bad
function q() {}

// good
function query() {}
```

Use camelCase for objects, functions, namespaces (TS), and instances. Single words should be lowercased. eslint: [`camelcase`](https://eslint.org/docs/rules/camelcase.html)

```javascript
// bad
function MyFunction() {}
const my_object = {};

// good
function myFunction() {}
const myObject()  = {};
```

Use PascalCase for naming classes, enums (TS), interfaces (TS) and constructors. eslint: [`new-cap`](https://eslint.org/docs/rules/new-cap.html)

```javascript
// bad
function user(options) {}
class user {}
class myClass {}

// good
class User {}
class MyClass {}
```

Do not prefix interfaces in typescript

```typescript
// bad
interface IMyInterface {}

// good
interface MyInterface {}
```

**[⬆ back to top](#table-of-contents)**

## Comments

Use `/** ... */` for a comments block (multiline).

```javascript
// bad
// calc() will return a number
// based on input
//
// @param {number} num
function calc(num) {
  return num + 1;
}

// good
/**
 * calc() will return a number
 * based on input
 *
 * @param {number} num
 */
function calc(num) {
  return num + 1;
}
```

Use `//` for a single line comment. Place single line comments on a newline **above** the subject of the comment.

```javascript
// bad
const param = 1; // assign 1 to param

//good

// assign 1 to param
const param = 1;
```

Allow empty line above single line comment (`//`), and start comments with a space. eslint: [spaced-comment](https://eslint.org/docs/rules/spaced-comment)

```javascript
// bad
//assign 1 to param
const param = 1;

// good
// assign 1 to param
const param = 1;

// bad
/**
 *calc() will return a number
 *based on input
 *
 *@param {number} num
 */
function calc(num) {
  return num + 1;
}

// good
/**
 * calc() will return a number
 * based on input
 *
 * @param {number} num
 */
function calc(num) {
  return num + 1;
}
```
**[⬆ back to top](#table-of-contents)**
# ProductiveHub JavaScript Style Guide() {

ProductiveHub official JavaScript (and TypeScript ) styleguide.

## Table of Contents

1. [Naming Conventions](#references)

**[⬆ back to top](#table-of-contents)**

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
interface IMyInterface {};

// good
interface MyInterface {};
```

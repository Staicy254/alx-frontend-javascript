# ECMAScript 6 (ECMAScript 2015) Features

This repository is a comprehensive guide and collection of examples for some of the key features introduced in ECMAScript 6 (also known as ECMAScript 2015). The topics covered include statements and declarations, arrow functions, default parameters, rest parameters, and an in-depth look at iterables and iterators.

## Table of Contents
- [Statements and Declarations](#statements-and-declarations)
- [Arrow Functions](#arrow-functions)
- [Default Parameters](#default-parameters)
- [Rest Parameter](#rest-parameter)
- [Demystifying ES6 Iterables & Iterators](#demystifying-es6-iterables--iterators)

## Statements and Declarations
ES6 introduced new ways to declare variables and constants, making the language more predictable and reducing common pitfalls associated with variable scoping.

### Examples:
- `let` and `const` for block-scoped variable and constant declaration.
- `class` syntax for defining classes.
- `import` and `export` statements for module management.

## Arrow Functions
Arrow functions provide a shorter syntax for writing functions and lexically bind the `this` value, making them more concise and easier to work with in certain contexts.

### Examples:
```javascript
// Traditional function expression
function add(a, b) {
  return a + b;
}

// Arrow function
const add = (a, b) => a + b;

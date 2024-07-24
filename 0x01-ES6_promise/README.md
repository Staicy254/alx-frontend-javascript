# JavaScript Promises and Asynchronous Programming

## Introduction
This guide provides an overview of JavaScript Promises and asynchronous programming concepts, including `Promise`, `async/await`, and error handling with `try/catch`. These tools are essential for managing asynchronous operations, such as API calls, file I/O, and timers, in JavaScript.

## Table of Contents
1. [Promise](#promise)
2. [Async and Await](#async-and-await)
3. [Error Handling: Try and Catch](#error-handling-try-and-catch)

## Promise
A `Promise` in JavaScript represents an operation that hasn't completed yet, but is expected in the future. It's an object that can be in one of three states:

- **Pending:** The initial state, neither fulfilled nor rejected.
- **Fulfilled:** The operation completed successfully.
- **Rejected:** The operation failed.

### Basic Syntax
```javascript
let promise = new Promise((resolve, reject) => {
    // Asynchronous operation
    if (/* success */) {
        resolve('Success');
    } else {
        reject('Error');
    }
});

promise.then(result => {
    console.log(result);
}).catch(error => {
    console.error(error);
});

Async and Await
async and await are syntactic sugar over promises, making asynchronous code easier to write and read.

async: This keyword is used to declare an asynchronous function, which returns a promise.
await: This keyword is used to wait for a promise to resolve or reject. It can only be used inside an async function.

async function fetchData() {
    try {
        let response = await fetch('url');
        let data = await response.json();
        console.log(data);
    } catch (error) {
        console.error(error);
    }
}

fetchData();

Error Handling: Try and Catch
When using async/await, errors can be handled using try/catch blocks. This approach helps in managing exceptions and makes the code more readable.

async function exampleFunction() {
    try {
        let result = await asyncOperation();
        console.log(result);
    } catch (error) {
        console.error('Error:', error);
    }
}

exampleFunction();


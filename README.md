# Exercise-8.10-Array-Map

Springboard SE Bootcamp - Array Map Exercise for Section 8.10

Assignment Instructions: https://lessons.springboard.com/Array-Methods-map-Exercise-22bff432872144dabea471707531625c

## Recall: What is a Callback Function?

A **callback function** is a function that is **passed as an argument** to another function and is **invoked** (called back) at a later time.

In JavaScript, callbacks are used extensively in built-in methods.

### callback example:

```js
function greet(name) {
  console.log(`Hello, ${name}!`);
}

function processUserInput(callback) {
  const name = "Alice";
  callback(name); // Call the passed-in function
}

processUserInput(greet); // Output: Hello, Alice!
```

In this example:

- `greet` is passed as a **callback** to `processUserInput`.
- `processUserInput` calls `greet` with the name `"Alice"`.

## What is the map() Method?

The `map()` method is an **array method** in JavaScript used to **transform each element** in an array and return a **new array** with the transformed values.

### simple Array.map example

```js
const numbers = [1, 2, 3];
const doubled = numbers.map(function (num) {
  return num * 2;
});

console.log(doubled); // Output: [2, 4, 6]
```

Notes:

- `map()` does **not** modify the original array.
- It always returns a **new array**.
- It’s commonly used for transforming or formatting data (or extracting out values from complex data objects in an array).

### Summary - When to Use Callbacks and map()

- Use **callbacks** when you want to pass custom behavior into a function.
- Use `map()` when you need to **transform an array** into a new one based on existing values.

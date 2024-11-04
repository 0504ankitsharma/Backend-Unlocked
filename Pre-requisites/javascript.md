## Variables in JavaScript

Variables in JavaScript are used to store and manipulate data. There are three main ways to declare variables in JavaScript:

1. **`var`** - This is the original way to declare variables in JavaScript. Variables declared with `var` are function-scoped, meaning they are accessible within the function they are defined in. If declared outside of a function, they are global.

```javascript
function example() {
  var x = 5;
  console.log(x); // Output: 5
}

example();
console.log(x); // Error: x is not defined
```

2. **`let`** - `let` is the recommended way to declare variables in modern JavaScript. Variables declared with `let` are block-scoped, meaning they are accessible within the block (e.g., a pair of curly braces `{}`) they are defined in.

```javascript
if (true) {
  let y = 10;
  console.log(y); // Output: 10
}

console.log(y); // Error: y is not defined
```

3. **`const`** - `const` is used to declare variables that are meant to be constant, meaning their value cannot be reassigned. `const` variables are also block-scoped like `let`.

```javascript
const PI = 3.14;
PI = 3.15; // Error: Assignment to constant variable.

if (true) {
  const z = 15;
  console.log(z); // Output: 15
}

console.log(z); // Error: z is not defined
```

The main differences between `var`, `let`, and `const` are:
- **Scope**: `var` is function-scoped, `let` and `const` are block-scoped.
- **Reassignment**: `var` and `let` variables can be reassigned, `const` variables cannot.
- **Hoisting**: `var` variables are hoisted (can be accessed before declaration), `let` and `const` are not.

It's generally recommended to use `let` for variables that need to be reassigned, and `const` for variables that are meant to be constant. This helps you better manage the state of your application.

## Data Types in JavaScript

JavaScript has several built-in data types:

1. **Primitive Data Types**:
   - **String**: Represents text, e.g., `"Hello, world!"`.
   - **Number**: Represents both integers and floating-point numbers, e.g., `42`, `3.14`.
   - **Boolean**: Represents a logical value, either `true` or `false`.
   - **Undefined**: Represents a variable that has been declared but has not yet been assigned a value.
   - **Null**: Represents the intentional absence of any object value.
   - **Symbol**: Represents a unique and immutable identifier.

2. **Non-Primitive Data Types**:
   - **Object**: Represents a collection of key-value pairs, e.g., `{ name: "John", age: 30 }`.
   - **Array**: Represents an ordered collection of values, e.g., `[1, 2, 3, 4, 5]`.
   - **Function**: Represents a reusable block of code that can be called with arguments and can return a value.

You can check the data type of a variable using the `typeof` operator:

```javascript
console.log(typeof "Hello");       // Output: "string"
console.log(typeof 42);            // Output: "number"
console.log(typeof true);          // Output: "boolean"
console.log(typeof undefined);     // Output: "undefined"
console.log(typeof null);          // Output: "object" (this is a known bug in JavaScript)
console.log(typeof {});            // Output: "object"
console.log(typeof []);            // Output: "object"
console.log(typeof function() {}); // Output: "function"
```

Understanding variables and data types is crucial for managing the state of your application and working with data in Node.js, Express, and MongoDB. Let me know if you have any other questions!
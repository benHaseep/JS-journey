2023-05-24
[link](https://www.youtube.com/watch?v=9O0oCER-vLo&list=PLknwEmKsW8OuTqUDaFRBiAViDZ5uI3VcE&index=39)

---

> let released in EcmaScript 2015.

```js
for (var i = 0 ; i < 10 ; i++) {

}
console.log(i); // 10
// cuz `var i;` hoisted and became a global variable.

for (let x = 0 ; x < 10 ; x++) {

}
console.log(x); // error: Uncaught ReferenceError: x is not defined.
// cuz let isn't hoisted, so it's still local variable.

```


self invoked function:
```js
function hello () {
	console.log(`Hello, World!`);
}
hello();  // Hello, World!

(function () {
	console.log(`Hello, World!`);
}) ();  // Hello, World!
```

The importance of self invoked functions is to discard any conflicts in global variables.
```js

(function () {
	console.log(`Hello, World!`);
	var x = 1
	let y = 2
	console.log(`Hello, World!`);
})();

console.log(x); // error: Uncaught ReferenceError: x is not defined.
console.log(y); // error: Uncaught ReferenceError: x is not defined

// in this code you are using the variables you need in your local scope so your variables don't conflict the variables created from others.

```

[[Microsoft quiz]]
### Self invoke explaination from ChatGPT

In JavaScript, self-invoked functions, also known as immediately invoked function expressions (IIFE), are functions that are executed immediately after they are defined. They are commonly used to create a local scope for variables and functions, preventing them from polluting the global scope.

Here's the basic syntax of a self-invoked function:
```javascript
(function() {
  // Function body
})();
```

Let's break down how a self-invoked function works:

1. Function declaration:
   `(function() { ... })` creates an anonymous function declaration. The function can also have parameters if needed, like `(function(param1, param2) { ... })(value1, value2)`.

2. Invocation:
   Following the function declaration, we append `()` at the end to immediately invoke the function.

3. Execution:
   The function is executed immediately after it is defined. It runs its code block, performing any operations or calculations as defined within the function body.

Self-invoked functions are often used to encapsulate code and create a private scope. Variables and functions defined within the self-invoked function are not accessible from the outside, protecting them from conflicting with other variables and functions in the global scope.

Here's an example to illustrate how self-invoked functions can be used:

```javascript
(function() {
  var x = 10;
  var y = 5;
  
  function add(a, b) {
    return a + b;
  }
  
  var result = add(x, y);
  console.log(result); // Output: 15
})();

console.log(x); // Throws an error: x is not defined
console.log(y); // Throws an error: y is not defined
console.log(add); // Throws an error: add is not defined
```

In this example, the variables `x` and `y`, as well as the function `add`, are defined within the self-invoked function's scope. They are not accessible outside of the function, indicated by the errors thrown when trying to access them. The self-invoked function creates a self-contained environment for the variables and functions it declares, ensuring they don't interfere with other parts of the code.

Self-invoked functions are commonly used in JavaScript modules, as they allow for the encapsulation of code and the creation of private variables and functions that are only accessible within the module.
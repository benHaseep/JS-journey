2023-05-24
[link](https://www.youtube.com/watch?v=-pHfultSrKY&list=PLknwEmKsW8OuTqUDaFRBiAViDZ5uI3VcE&index=38)

-----
```js
hello() // Hello Wrold!

function hello () {
	console.log("Hello Wrold!");
}

// this is declaration type of functions.
// the Intrepreter read this code like this:

/*
function hello () {
	console.log("Hello Wrold!");
}
hello()
*/

// in js the variables (var) and the declaration functions is hoisted to the top.

```

```js
hello() // error: Uncaught ReferenceError: can't access lexical declaration 'hello' before

let hello = function () {
	console.log("Hello Wrold!");
}

// this expression type of functions.
// the Intrepreter read this code like this:
/*
hello()
function hello () {
	console.log("Hello Wrold!");
}
*/
// in js the variables (let) and the expression functions isn't hoisted to the top.
```
### ChatGPT hoisting explaination
In JavaScript, hoisting is a mechanism that allows variables and function declarations to be moved to the top of their containing scope during the compilation phase, before the code is executed. This means that regardless of where variables and functions are declared in the code, they are conceptually moved to the top of their scope.

It's important to note that hoisting affects the declarations themselves, not the initializations or assignments. Let's look at two common cases: hoisting of variable declarations and hoisting of function declarations.

1. Variable Hoisting:
When a variable is declared using the `var` keyword, the declaration is hoisted to the top of its scope. However, only the declaration is hoisted, not the initialization.

For example:
```javascript
console.log(x); // Output: undefined
var x = 5;
console.log(x); // Output: 5
```

In the above example, even though `x` is referenced before it's assigned a value, it doesn't throw an error. This is because the variable declaration `var x` is hoisted to the top of the scope, resulting in `x` being defined but uninitialized at the point of the first `console.log()` statement.

2. Function Hoisting:
Function declarations are also hoisted to the top of their scope. This means that you can call a function before its declaration in the code.

For example:
```javascript
foo(); // Output: "Hello"
function foo() {
  console.log("Hello");
}
```

In this case, the function `foo` is hoisted to the top of its scope, so it can be called before its actual declaration.

It's important to note that hoisting applies only to function declarations, not function expressions. Function expressions are not hoisted and must be declared before they are used.

For example:
```javascript
foo(); // Throws an error: foo is not a function
var foo = function() {
  console.log("Hello");
};
```

In this case, the variable `foo` is hoisted to the top of its scope, but since it's initialized with a function expression and not a function declaration, it results in an error when we try to call it.

To avoid confusion and improve code readability, it's generally recommended to declare variables at the top of their scope and define functions before they are used, even though hoisting allows you to do otherwise.
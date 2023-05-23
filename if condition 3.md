2023-05-23

----

New way to write if statement.
condition ?
	code
:condition
	code
:code
```js
let age = prompt("What is your age?")

  

age > 18 ?    // if
	document.write("Hello, user")
:age == 18 ?  // else if
	document.write("You are 18 now. Hello")
:document.write("No you are very young");  // else
```

you can save the result in a variable
```js
let age = prompt("What is your age?")

  

let result = age > 18 ?

"Hello, user"

:age == 18 ?

"You are 18 now. Hello"

:"No you are very young";

  

console.log(result);
```

you can write it on one line:
```js
let age = prompt("What is your age?")

let result = age > 18 ? "Hello, user" :age == 18 ? "You are 18 now. Hello" :"No you are very young";

console.log(result);
```


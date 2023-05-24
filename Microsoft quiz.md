

```js

console.log( x() );
function x () {
	function y () { return 1 };
	return y();
	function y () { return 0 }
}

// the answer choices (1, 0, error)

```

### the answer:
```js
// the correct answer is (0)
// cuz the intrepreter read this code like this:

function x () {
	function y () { return 1 };
	function y () { return 0 };
	return y();
}
console.log( x() ); // 0
```

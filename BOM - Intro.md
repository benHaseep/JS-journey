2023-05-28

----

BOM -> Browser Object Model

- Window
	- document
		- body
	- console
		- log

```js
document.write("Hello from document") // Hello from document
window.document.write("Hello from document") // Hello from document

console.log("Hello from console"); // Hello from console
window.console.log("Hello from console"); // Hello from console

function hello () {
	console.log("Hello!");
}
hello() // Hello!
window.hello() // Hello!



```


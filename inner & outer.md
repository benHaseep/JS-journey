2023-05-25

----

```html
<body>

	<div class="container">
		<h3>Hello world</h3>
	</div>

</body>
```
```js
let container = document.getElementById('container')

console.log(container.outerHTML);
/*
<div id="container">
	<h3>Hello world</h3>
</div>
*/11
console.log(container.innerHTML); // <h3>Hello world</h3>
```
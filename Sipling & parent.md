2023-05-25

----

```html
<div id="container">
	<h3 id="first">First</h3>
	<h3 id="second">Second</h3>
	<h3 id="third">Third</h3>
</div>
```
```js
let element = document.getElementById('second');

console.log(element); // <h3 id="second">
console.log(element.previousElementSibling); // <h3 id="first">
console.log(element.nextElementSibling); // <h3 id="third">

console.log(element.parentElement); // <div id="container">
```
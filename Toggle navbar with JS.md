2023-05-28

----

```html
<button id="open" class="hide">Open</button>
<button id="close">Close</button>

<div class="container">
	<p>Home</p>
	<p>Courses</p>
	<p>News</p>
	<p>Problem Solving</p>
	<p>Quizes</p>
	<p>Blogs</p>
	<p>Chats</p>
</div>
```
```css
* {
	margin: 0;
}

button {
	border: none;
	background-color: coral;
	color: #fff;
	border-radius: 5px;
}

.container {
	width: 180px;
	height: 100vh;
	background-color: coral;
	color: #fff;
}

.container p {
	padding: 5px;
}

.container p:hover, button:hover {
	background-color: #000;
	cursor: pointer;
}

#close {
	position: absolute;
	left: 185px;
}

.hide {
	display: none;
}
```
```js
let btnOpen = document.getElementById('open');
let btnClose = document.getElementById('close');
let container = document.querySelector('.container');

btnClose.onclick = () => {
	btnOpen.classList.toggle('hide');
	btnClose.classList.toggle('hide');
	container.classList.toggle('hide');
}

btnOpen.onclick = () => {
	btnOpen.classList.toggle('hide');
	btnClose.classList.toggle('hide');
	container.classList.toggle('hide');
}
```

[the result](https://codepen.io/benHaseep/pen/mdzgoRa)
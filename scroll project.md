2023-05-29

----

```html
<button id="btn">^</button>
```
```css
body {
	height: 2000px;
	width: 2000px;
}

#btn {
	width: 20px;
	height: 20px;
	background-color: #fa0;
	border: none;
	position: fixed;
	bottom: 20px;
	right: 20px;
	display: none;
	cursor: pointer;
}

```
```js
let btn = document.getElementById('btn');

window.onscroll = () => {
	if (scrollY >= 400) {
		btn.style.display = "block"
	} else {
		btn.style.display = "none"
	}
}

btn.onclick = () => {
	scrollTo({
		top:0,
		left:0,
		behavior:"smooth"
	})
}
```

[the result](https://codepen.io/benHaseep/pen/YzJMbwN)


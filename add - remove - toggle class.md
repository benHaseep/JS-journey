2023-05-28

----

### add & remove class:
```html
<p id="hello">Hello!</p>
```
```css
.test {
	background-color: #000;
	padding: 10px;
	color: #fff;
}
```
```js
let hello = document.getElementById('hello');


hello.onclick = () => {
	hello.classList.add("test")
};

hello.oncontextmenu = () => {
	hello.classList.remove("test")
};
```
[the result](https://codepen.io/benHaseep/pen/oNaOdBK)


### toggle class:
```html
<p id="hello">Hello!</p>
```
```css
.test {
	background-color: #000;
	padding: 10px;
	color: #fff;
}
```
```js
let hello = document.getElementById('hello');


hello.onclick = () => {
	hello.classList.toggle("test")
};
```
[the result](https://codepen.io/benHaseep/pen/poxBVea)



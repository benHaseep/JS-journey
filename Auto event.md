2023-05-28

----


```html
<input type="text" id="txt" placeholder="Open">
<button id="btn">Click</button>
```
```js
let txt = document.getElementById('txt');
let btn = document.getElementById('btn');

window.onload = () => {
	txt.focus()
	txt.value = "Test"
}
```

[the result](https://codepen.io/benHaseep/pen/KKGYEoM)


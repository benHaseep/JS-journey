2023-05-28

----



```html
<button id="after">After</button>
<button id="before">Before</button>
<button id="append">Append</button>

<p id="content">Content</p>

<div id="container"></div>
```
```js
let after = document.getElementById('after');
let append = document.getElementById('append');
let before = document.getElementById('before');

let content = document.getElementById('content');
content.style.color = "blue"

let container = document.getElementById('container');
container.style.backgroundColor = "#ffa";
container.style.height = "50px";


after.onclick = () => {
	container.after(content)
};

before.onclick = () => {
	container.before(content)
};

append.onclick = () => {
	container.append(content)
};

```

[the result](https://codepen.io/pen/)

2023-05-30
local storage & session storage project.

----

```html
<input type="text" id="name" placeholder="Name">
```
```js
let name = document.querySelector('#name');
// select the input element.

name.onkeyup = () => {
	localStorage.name = name.value;
}
// get the date from the form and sotre it in local sotarge.

name.value = localStorage.name;
// data from local storage to the form.
```


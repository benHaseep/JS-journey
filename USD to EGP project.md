2023-05-28

-----

```html
<input type="number" placeholder="USD" id="dollar">
<input type="number" placeholder="EGP" id="pound">
```
```js
let dollar = document.getElementById('dollar');
let pound = document.getElementById('pound');

dollar.onkeyup = function () {
	pound.value = dollar.value * 30.85;
};

pound.onkeyup = function () {
	dollar.value = pound.value / 30;
};
```



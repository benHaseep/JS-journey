2023-05-25

----


```js
let user = {
	name: "Ali",
	getName:function () {
		return this.name;
		// = return user.name;
	}
}
console.log(user.getName()); // Ali
```

```js
let x = this;
console.log(x); // Window

```

```js
function hello () {
	return this;
}
console.log(hello()); // Window
```

in strict mode:
```js
"use strict";
function hello () {
	return this;
}
console.log(hello()); // undefined
```


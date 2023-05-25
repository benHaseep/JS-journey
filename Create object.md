2023-05-25

----

```js
let user = {};
user.name = "Ali";
// here you added key (name) and give it value (Ali)
console.log(user); // Object { name: "Ali" }
```

```js
let user = {
	name: "Ahmed",
};
user.name = "Ali";
// here you modified the name from (Ahmed) to (Ali)
console.log(user.name); // Ali
```

```js
let user = {
	name: "Ahmed",
};

user.age = 21
// here we added age property and give it (21)
console.log(user.age); // 21
```

```js
let user = {
	name: "Ahmed",
};

user.hello = function () {
	return "Hello"
}

// here we added age hello property its value is a function
console.log(user.hello()); // Hello
```
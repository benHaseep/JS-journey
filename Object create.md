2023-05-25

---------

`Object.create()` -> copies data from object to another one.
the syntax:
`let newObject = Object.create(oldObject)`

```js
let user1 = {
name: "Ali",

getName: function () {
	return `Hello, ${user1.name}`
	},
}

let user2 = Object.create(user1);

console.log(user2.name); // Ali
console.log(user2.getName()); // Hello, Ali
```

modify data in the new object:
```js
let user1 = {
	name: "Ali",
	getName: function () {
		return `Hello, ${user1.name}`
	}
}

let user2 = Object.create(user1);
user2.name = "Moaz"
console.log(user2.name); // Moaz
console.log(user2.getName()); // Hello, Ali
// there is problem. we modified the user2.name and the method still give use the old name.
// `this` -> solve this problem.
```

this -> solves you problem.
```js
let user1 = {
	name: "Ali",
	getName: function () {
		return `Hello, ${this.name}`
	}
}

let user2 = Object.create(user1);
user2.name = "Moaz"

console.log(user2.name); // Moaz
console.log(user2.getName()); // Hello, Moaz
```


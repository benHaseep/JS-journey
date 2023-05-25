2023-05-25

---

In JavaScript, the `Object.assign()` function copies properties from one or more source objects to a target object. It returns the target object.

the syntax: 
`let newObject = Object.assign(oldObject, old Object2,...)`

Here is an example of how to use it:
```js
let a1 = {
	num1: 1,
	hello: function() {
		return `Hello`
	},
}
let a2 = {
	num2: 2,
}

let a3 = {
	num3: 3
}

let a4 = Object.assign(a1)
console.log(a4); // { num1: 1, hello: hello() }

a4 = Object.assign(a1, a2)
console.log(a4); // Object { num1: 1, hello: hello(), num2: 2 }

a4 = Object.assign(a1, a2, a3)
console.log(a4); // { num1: 1, hello: hello(), num2: 2, num3: 3 }

a4.num1 = 10;
console.log(a4.num1); // 10
```


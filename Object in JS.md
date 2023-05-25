2023-05-24

---

```js
let x = { }
console.log(typeof x); // object
```

```js
let car = {
	title: "Tyota",
	price: 100000,
	color: ["white", "grey", "black"],
	model: 2020,
	hello: function () {
		return "Hello";
		}
}

console.log(car); // Object { title: "Tyota", price: 100000, color: "Grey", model: 2020, hello: hello() }
console.log(car.title);    // Tyota
console.log(car.color);    // [ "white", "grey", "black" ]
console.log(car.color[2]); // black
console.log(car.hello);    // function hello()
console.log(car.hello());  // Hello
```

[[Nested object]]
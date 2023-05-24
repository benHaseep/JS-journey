2023-05-24
[link](https://www.youtube.com/watch?v=cCSsnlb59UA&list=PLknwEmKsW8OuTqUDaFRBiAViDZ5uI3VcE&index=40)

---
```js
function x (parameter) {
	
}
x(arguments);
```

the default value for the parameter if you don't give it value is `undefined` 
```js
function hello (name) {
	console.log(`hello, ${name}`);
}
hello("Ali"); // hello, Ali
hello(); // hello, undefined
//the default value for the parameter if you don't give it value is `undefined` 
```

changing the default parameter value:
```js
function hello (name="User") {
	console.log(`Hello, ${name}`);
}
hello("Ali"); // hello, Ali
hello(); // hello, User
// notice, the default value changed from undefined to User.
```


```js
function calcAge(age) {
	console.log(age * 356);
}
calcAge(21); // 7476
calcAge(); // NaN
```
```js
function calcAge(age=0) {
	console.log(age * 356);
}
calcAge(21); // 7476
calcAge(); // 0
```

make an array parameter and add all the numbers 
```js
function calc ( ...nums ) {
	// ...nums means -> empty array [ ] named nums
	let result = 0
	for (let i = 0 ; i < nums.length ; i++) {
		result += nums[i];
}
	console.log(result);
}
calc(5) // 5
calc(5, 5) // 10
calc(23,24,4252,45,345,345,543) // 5577
```
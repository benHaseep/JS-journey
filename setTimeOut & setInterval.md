2023-05-29

----


**Set Time Out:**
The `setTimeout()` method calls a function after a number of milliseconds.
1 second = 1000 milliseconds
```js
setTimeout(() => {
	console.log(`Hello`);
}, 3000);
// "Hello" shown in the console after 3 seconds
```

**Clear Time Out:**
The `clearTimeout()` method clears a timer set with the `setTimeout()` method.
```js
let hello = setTimeout(() => {
	console.log(`Hello`);
}, 3000);

clearTimeout(hello);
// the function doesn't run after the 3s
```

**Set Time Interval**
The `setInterval()` method calls a function at specified intervals (in milliseconds).
The `setInterval()` method continues calling the function until `clearInterval()` is called, or the window is closed.
1 second = 1000 milliseconds.
```js
let i = 0;

let hello = setInterval(()=>{
	console.log(i++);
}, 1000);
// the function runs every 1s.
```

**Clear Interval:**
The `clearInterval()` method clears a timer set with the `setInterval()` method.
```js
let i = 0;

let hello = setInterval(()=>{
	console.log(i++);
}, 1000);

clearInterval(hello);
// the function doesn't run after the 1s
```



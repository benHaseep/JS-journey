2023-05-24

----

```js
function pro(price, taxes, ads) {
	let product = price + taxes;
	let result = product + ads;
	return result;
}

pro(200, 3, 10); // nothing
pro(400, 4, 34); // nothing
pro(500, 2, 32); // nothing

let x = pro(500, 2, 32);
console.log(x); // 534
// return value is the function value.
// return let you use the result of any function in other places.
// the return is the last line in the function, interpreter  can't read anything under the return.
```

```js
function x () {
	return 100;
}
console.log(x()); // 100
```

```js
function calcAgeByDays (age) {
	return age * 365;
}
let days = calcAgeByDays(21);

function calcAgeByHours (days) {
	return days * 24;
}
let hours = calcAgeByHours(days);

console.log(`${hours} hours`); // 183960 hours

```


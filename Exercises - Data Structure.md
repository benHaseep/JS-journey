2023-06-06

-----
### The sum of a range
The introduction of this book alluded to the following as a nice way to
compute the sum of a range of numbers:
console.log(sum(range(1, 10)));
Write a range function that takes two arguments, start and end, and
returns an array containing all the numbers from start up to (and
including) end.
Next, write a sum function that takes an array of numbers and returns
the sum of these numbers. Run the example program and see whether
it does indeed return 55.
As a bonus assignment, modify your range function to take an optional third argument that indicates the “step” value used when building the array. If no step is given, the elements go up by increments
of one, corresponding to the old behavior. The function call range(1,
10, 2) should return `[1, 3, 5, 7, 9]`. Make sure it also works with
negative step values so that range(5, 2, -1) produces `[5, 4, 3, 2]`.

```js
function range (start, end, step=1) {

let result = []

	if (start < end) {
		for (let i = start; i <= end; i += step) {result.push(i)}
	} else {
		for (let i = start; i >= end; i -= step) {result.push(i)
	}

	return result;
}

console.log(range(1,10)) // [ 1, 2, 3, 4, 5, 6, 7, 8, 9, 10 ]
console.log(range(1, 10, 2)); // [ 1, 3, 5, 7, 9 ]
console.log(range(10, 1, 2)); // [ 10, 8, 6, 4, 2 ]

function sum (nums) {
	let result = 0;
	for (let n of nums) {result += n};
	return result;
}

console.log(sum(range(1,10))); // 55

```

### Reversing an array
Arrays have a reverse method that changes the array by inverting the
order in which its elements appear. For this exercise, write two func-
tions, reverseArray and reverseArrayInPlace. The first, reverseArray,
takes an array as argument and produces a new array that has the
same elements in the inverse order. The second, reverseArrayInPlace,
does what the reverse method does: it modifies the array given as argu-
ment by reversing its elements. Neither may use the standard reverse
method.
Thinking back to the notes about side effects and pure functions in
the previous chapter, which variant do you expect to be useful in more
situations? Which one runs faster?

```js
function reverseArray (arr) {

	let result = [];
	for (let i = arr.length -1 ; i >= 0; i--) {
		result.push(arr[i])
	}
	return result
}

console.log(reverseArray(['a', 'b', 'c'])); // [ 'c', 'b', 'a' ]

```

```js
function reverseArrayInPlace (arr) {

let result = [];

for (let i = 0; i < arr.length; i++) {result.unshift(arr[i])}

for (let i = 0; i < result.length; i++) {
		arr.push(result[i]);
		arr.shift()
	}
}

let arrayValue = [1, 2, 3, 4, 5];
reverseArrayInPlace(arrayValue);
console.log(arrayValue);
// [ 5, 4, 3, 2, 1 ]
```



###
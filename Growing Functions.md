2023-06-05

----

```js
function printFarmInventory(cows, chickens) {

// convert parameters from nums to string to concatinate 0s before it
	let cowString = String(cows);
	let chickenString = String(chickens);

// loop to concatinate 0s
	while (cowString.length < 3) {cowString = '0' + cowString;}
	while (chickenString.length < 3) {chickenString = '0' + chickenString}

// print the result
	console.log(`${cowString} Cows`);
	console.log(`${chickenString} Chickens`);
}

printFarmInventory(10, 30);
```

Make it better:
```js
function printZeroPadWithLable (number, label) {

	let numberString = String(number);
	while (numberString.length < 3) {numberString = '0' + numberString}
	console.log(`${numberString} ${label}`);
}

function printFarmInventory (cows=0, chickens=0, horses=0) {
	printZeroPadWithLable(cows, "Cows");
	printZeroPadWithLable(chickens, "Chickens");
	printZeroPadWithLable(horses, "Horses");
}

printFarmInventory(10, 100, 3);

```


Better:
```js

function zeroPad(number, width) {
	let string = String(number);
	while (string.length < width) {string = `0` + string}
	return string
}

function printFarmInventory (cows=0, chickens=0, horses=0) {
	console.log(`${zeroPad(cows, 3)} "Cows"`);
	console.log(`${zeroPad(chickens, 3)} "Chickens"`);
	console.log(`${zeroPad(horses, 3)} "Horses"`);
}

printFarmInventory(10, 100, 3)
```

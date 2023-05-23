2023-05-23

------

```js
let cars = ["BMW" , "Mercedes" , "Honda"];
let models = [ 2020 , 2021 , 2022];

for (let i = 0 ; i < cars.length ; i++) {
	console.log(`Car ${cars[i]}`);
	for (let i = 0 ; i < models.length ; i++) {
		console.log(`Model: ${models[i]}`);
}
console.log(`---------------`);
}

// Car BMW
// Model: 2020
// Model: 2021
// Model: 2022
// ---------------
// Car Mercedes
// Model: 2020
// Model: 2021
// Model: 2022
// ---------------
// Car Honda
// Model: 2020
// Model: 2021
// Model: 2022
// ---------------
```
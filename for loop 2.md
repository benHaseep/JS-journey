2023-05-23

-----

loop on array:
```js
let names = ["Ali", "John", "Moaz", "Haseep", "Gabr"];
  

for (let i = 0 ; i < names.length ; i++) {
	console.log(names[i]);
}
// Ali
// John
// Moaz
// Haseep
// Gabr
```


you can loop on stirng cuz it is a sequence value.
```js
let name = "benHaseep";

for (let i = 0 ; i < name.length ; i++) {
	console.log(name[i]);
}
// b
// e
// n
// H 
// a 
// s
// e
// e
// p
```

reverse loop:
```js
let names = ["Ali", "John", "Moaz", "Haseep", "Gabr"];

for (let i = names.length - 1 ; i >= 0 ; i--) {
	console.log(names[i]);
}
// Gabr
// Haseep
// Moaz
// John
// Ali
```
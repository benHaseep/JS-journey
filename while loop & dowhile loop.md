2023-05-23

-----

while:
```js
let i = 0;

while (i < 3) {
	console.log("Hello World!");
	i++
}
// Hello World!
// Hello World!
// Hello World!
```

dowhile:
```js
let i = 0;

do {
	console.log("Hello World!");
	i++
}while(i < 3)
// Hello World!
// Hello World!
// Hello World!
```

the diffrence between them:
```js

let i = 3;
while (i < 3) {
	console.log("Hello World!")
	i++
}
// nothing
```
```
let i = 3;

do {
	console.log("Hello World!");
	i++
}while(i < 3)
// Hello World!
```
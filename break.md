2023-05-23

----
```js
let users = [ "Ali" , "Mazen" , 1,2,3 , "Gamal" ];

for (let i = 0 ; i < users.length ; i++) {
	if (users[i] == "Mazen") {
		break
	}
	console.log(users[i]);
}
// Ali
```

```js
let users = [ "Ali" , "Mazen" , 1,2,3 , "Gamal" ];

for (let i = 0 ; i < users.length ; i++) {
	console.log(users[i]);
	if (users[i] == "Mazen") {
		break
	}
}
// Ali
// Mazen
```
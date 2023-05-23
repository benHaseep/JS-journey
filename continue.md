2023-05-23

----

Continue:
```js
let users = [ "Ali" , "Mazen" , 1,2,3 , "Gamal" ];

for (let i = 0 ; i < users.length ; i++) {
	if (typeof users[i] == "number") {
		continue
	}
	console.log(users[i]);
}

// Ali
// Mazen
// Gamal
```

```js
let users = [ "Ali" , "Mazen" , 1,2,3 , "Gamal" ];

for (let i = 0 ; i < users.length ; i++) {
	if (typeof users[i] != "number") {
		continue
	}
	console.log(users[i]);
}
// 1
// 2
// 3
```

```js
let users = [ "Ali" , "Mazen" , 1,2,3 , "Gamal" ];

for (let i = 0 ; i < users.length ; i++) {
	if (users[i] == "Mazen") {
		continue
	}
	console.log(users[i]);
}

// Ali
// 1
// 2
// 3
// Gamal
```

```js
let users = [ "Ali" , "Mazen" , 1,2,3 , "Gamal" ];

for (let i = 0 ; i < users.length ; i++) {
	if (users[i] != "Mazen") {
		continue
	}
	console.log(users[i]);
}
// Mazen
```


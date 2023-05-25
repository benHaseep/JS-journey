2023-05-24

----

```js
let user = {
	// properties
	firstName: "Mohamed",
	lastName: "Haseep",
	email: "benHaseep@outlook.com",
	age: 21,
	skill: ["HTML", "CSS", "JS"],
	active: true,
	phoneNumber: {
		mobile: 0123445667,
		home: 0876655443
	},
	adress: {
		Egypt: "Cairo",
		UAE: "Abu Dhabi"
	},
	// methods
	isActive: function () {
		if(user.active === true) {
		return `Hello ${user.firstName}`;
		}else {
		return `Sorry, you are not active.`;
	}
	},
	getAge: function() {
		if (user.age >= 18) {
		return `Available`;
		}else{
		return `Unavailable`;
		}
	},
}
console.log(user.firstName); // Mohamed
console.log(user["firstName"]); // Mohamed
console.log(user.phoneNumber.home); // 876655443
console.log(user["phoneNumber"]["home"]); // 876655443

console.log(user.isActive()); // Hello Mohamed
console.log(user.getAge()); // Available
console.log(user["getAge"]()); // Available
```


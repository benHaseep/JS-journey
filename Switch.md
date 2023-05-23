2023-05-23

----
```js
let role = prompt("What is your role?")

switch(role) {
	case "admin":
		document.write("admin")
		break
	case "moderator":
		document.write("moderator")
		break
	default:
		document.write("user")
}

// switch doesn't accept (>, <), it accepts == only.
```


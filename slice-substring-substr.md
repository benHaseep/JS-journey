2023-05-20

----

```js
let name = "Mohamed El-Sayed Haseep";

  

console.log(name.slice()); // Mohamed El-Sayed Haseep

console.log(name.substring()); // Mohamed El-Sayed Haseep

console.log(name.substr()); // Mohamed El-Sayed Haseep

// all of them make the same thing.

  

console.log(name.slice(-6)); // Haseep

console.log(name.slice(-6, -3)); // Has

  

console.log(name.substring(-6)); // Mohamed El-Sayed Haseep

console.log(name.substring(-6, -3)); // <empty string>

// substring doesn't accept a negative value.

  

console.log(name.substr(0, 7)); // Mohamed

console.log(name.substr(17, 6)); // Haseep

// substr(start, length)

  

// the three functions are used to cut from string.

// We often use slice.
```

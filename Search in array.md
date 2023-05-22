2023-05-22

----

indexOf: searching for the index of a value.
```js 
let names = [ "Ali", "John", "Moaz" ];

console.log(names.indexOf("Moaz")); // 2
console.log(names.indexOf("Moaz", 3)); // -1 -> -1 means not found.
// search for the index of "Moaz", start searching from index[3].
```

lastIndexOf: searching for the index of a value, but start searching from RTL.
```js
let names = [ "Ali", "John", "Moaz" ];

console.log(names.lastIndexOf("Moaz")); // 2
console.log(names.lastIndexOf("Moaz", 3)); // 2
// search for the index of "Moaz", start searching from index[3].
```

includes: 
```js
let names = [ "Ali", "John", "Moaz" ];

console.log(names.includes("Moaz")); // true
console.log(names.includes("Moaz", 3)); // flase
// search for the index of "Moaz", start searching from index[3].
```


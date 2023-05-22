
splice: deleting values from.
```js
let names = [ "Ali", "John", "Moaz" ];

names.splice(1, 2); // [ "Ali" ]
console.log(names);
// splice: delete values from array.
// splice(starting index, number of values u wanna del
```

```js
let names = [ "Ali", "John", "Moaz" ];

names.splice(1,2,"gabr", "said"); // "Ali", "gabr", "said" ]
console.log(names);
// from index [1] delete two values and add "gabr", "said"
```

slice: take a piece of the array
```js
let names = [ "Ali", "John", "Moaz" ];

let slice = names.slice(0, 2);
console.log(names); // [ "Ali", "John", "Moaz" ]
console.log(slice); // [ "Ali", "John" ]
// slice does not affect on the array but copies from it
```
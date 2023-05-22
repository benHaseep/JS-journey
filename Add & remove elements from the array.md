
unshift: add element to first index

```js
let names = [ "Ali", "John", "Moaz" ];

names.unshift('Haseep', 'said');
console.log(names); // [ "Haseep", "said", "Ali", "John", "Moaz" ]
// unshift: add values to the first index in the array
```

Push: add element to last index
```js
let names = [ "Ali", "John", "Moaz" ];

names.push('Haseep', 'said');
console.log(names); // [ "Ali", "John", "Moaz", "Haseep", "said" ]
// push: add values to last index in the array
```


shift: remove the first index in the array
```js
let names = [ "Ali", "John", "Moaz" ];

names.shift();
console.log(names); // [ "John", "Moaz" ]
// shift: remove the first value
```


pop: remove the last index in the array
```js
let names = [ "Ali", "John", "Moaz" ];

names.pop();
console.log(names); // [ "Ali", "John" ]
// shift: remove the last value
```


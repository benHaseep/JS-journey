2023-05-21

----

```js
let name = "benHaseep";

  
console.log(name.indexOf('e')); // 1
console.log(name.indexOf('e', 2)); // 6

console.log(name.lastIndexOf('e')); // 7
// indexOf: searching for a char and give you the index of the first one in the direction. -> (LTR)
// lastIndexOf: in the opposite dir.-> (RTL)

console.log(name.includes('a')); // true
console.log(name.includes('z')); // false

console.log(name.includes('n')); // true
console.log(name.includes('n', 3)); // false
```

```js
let name = "benHaseep";

console.log(name.startsWith('b')); // true
console.log(name.startsWith('z')); // false
// this function chech the start char of string

console.log(name.startsWith('n', 2)); // true
// is firt value is 'n', start from index 2.
// startsWith('value you search', index of starting)
```

```js
let name = "benHaseep";

console.log(name.endsWith('p')); // true
console.log(name.endsWith('eep')); // true
console.log(name.endsWith('z')); // false
// this function chech the end char of string.  

console.log(name.endsWith('n', 3));
// is last value of the first three values is 'n'?
// endsWith('the value U checking, the length you need to check in)
```
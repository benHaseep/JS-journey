2023-05-18

-----




```js
console.log('10' + '5');    // 105
console.log('10' - '5');    // 5
console.log('10' * '5');    // 50
console.log('10' / '5');    // 2

```

JavaScript converts numbers in strings `'10'` to Numbers `10` automatically in all calculations except add operation.
In add operation you should convert the Strings to Numbers manually.

### Method 1 to convert string to number
```js
console.log('5' + '5');      // 55
console.log(+'5' + +'5');    // 10

console.log(typeof '5');     // string
console.log(typeof +'5');    // number

console.log(+'5');         // 5
console.log(-'5');         // -5
console.log(-'-5') ;       // 5

console.log(+"Ali");       // NaN

console.log(+true);        // 1
console.log(+false) ;      // 0

console.log(+undefined);   // NaN
console.lgo(+null);// 0
```


[[4 Methods to convert strings to numbers]]
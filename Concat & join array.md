2023-05-22

----

```js
let names = [ "John", "Moaz", "Ali" ];

let nums = [4,3,2,1];

  

names += nums;

console.log(names); // John,Moaz,Ali4,3,2,1

console.log(typeof names); // string
```

concat: 
```js
let names = [ "John", "Moaz", "Ali" ];

let nums = [4,3,2,1];

  
  

console.log(names.concat(nums)); // [ "John", "Moaz", "Ali", 4, 3, 2, 1 ]

console.log(names.concat(nums, "haseep")); // [ "John", "Moaz", "Ali", 4, 3, 2, 1, "haseep" ]

// you can concat lots of arrays with strings and numbers.
```

join:
```js
let names = [ "John", "Moaz", "Ali" ];

  

console.log(names); // [ "John", "Moaz", "Ali" ]

console.log(names.join()); // John,Moaz,Ali

console.log(names.join('-')); // John-Moaz-Ali

console.log(typeof names.join()); // string
```
2023-05-20

----
### Repeat
```js
let str = "Ali "

console.log(str.repeat(2)); // Ali Ali
```

### length & charAt
```js
let str = "Ali";

console.log(str.length); // 3
// the string is a sequence value. Ali -> 'A','l','i'

let name = "benHaseep";
console.log(name.length); // 9

name[0]   //b
name[1]   //e
name[2]   //n

name.charAt(3)  //n

// ### the diffrence between [] and charAt.
name[10]   // undefined
name.charAt(10)   // 
// the CharAt() display does not display (undefined) when the index not founded.

```

### indexOf & lastIndexOf
indexOf: searching for a char and give you the index of the first one in the direction. -> (LTR)
lastIndexOf: in the opposite dir.-> (RTL)
```js
let name = "benHaseep";

// ### indexOf
console.log(name.indexOf('H'));
// indexOf () is a function that search for value in a sequence value.

console.log(name.indexOf('e'));

console.log(name.indexOf('e',3)); // starts searching from index[3]

// ### lastIndexOf
console.log(name.lastIndexOf('p')); // 8
// lastIndexOf() Searching in a sequence value
// starts searching form right to left.

console.log(name.lastIndexOf('H', 3)); //3
// search for 'H' but start searchin from index [-3]
```

### slice
```js
let name = "benHaseep";

console.log(name.slice()); // benHaseep

console.log(name.slice(3)); // Haseep
// slice the string from index 0 to the end of it.

console.log(name.slice(0,3)); // ben
// slice from index 0 to 3
// notice the index[3] is excluded.
```

### split
```js
let name = "Mohamed_El-Sayed_Haseep";

console.log(name.split()); // [ "Mohamed El-Sayed Haseep" ]
// split cuts the sequence value and store it in an array.

console.log(name.split('_')); // [ "Mohamed", "El-Sayed", "Haseep" ]

console.log(name.split('_', 2)); // [ "Mohamed", "El-Sayed" ]

console.log(name.split('')); // [ 'M', 'o', 'h', 'a', 'm', 'e', 'd', '_', 'E', 'l', '-', 'S', 'a', 'y', 'e', 'd', '_', 'H', 'a', 's', 'e', 'e', 'p']
```

[[slice-substring-substr]]
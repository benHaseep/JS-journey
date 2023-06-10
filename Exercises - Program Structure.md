


### Looping a triangle
Write a loop that makes seven calls to console.log to output the fol-
lowing triangle:
```
#
##
###
####
#####
######
#######
```


#### Answer:
```js
// Quiz 1

let rectangle = ''

for (let i = 0; i < 7; i++) {
	rectangle+='#';
	console.log(rectangle);
}
```





### FizzBuzz
Write a program that uses console.log to print all the numbers from 1
to 100, with two exceptions. For numbers divisible by 3, print "Fizz"
instead of the number, and for numbers divisible by 5 (and not 3), print
"Buzz" instead.
When you have that working, modify your program to print "FizzBuzz
" for numbers that are divisible by both 3 and 5 (and still print "Fizz"
or "Buzz" for numbers divisible by only one of those).
(This is actually an interview question that has been claimed to weed
out a significant percentage of programmer candidates. So if you solved
it, your labor market value just went up.)

#### Answer:
```js
// Quiz 2

for (let i = 1; i <= 100; i++) {
	if(i % 3 === 0) {console.log(`Fizz`)}
	else if (i % 5 === 0) {console.log(`Buzz`)}
	else {console.log(i)}
}
```



### Chessboard
Write a program that creates a string that represents an 8×8 grid, using
newline characters to separate lines. At each position of the grid there
is either a space or a "#" character. The characters should form a
chessboard.
Passing this string to console.log should show something like this:

```
 # # # #
# # # #
 # # # #
# # # #
 # # # #
# # # #
 # # # #
# # # #
```


#### Answer:
```js
// Quiz 3

let square = ' '

	for (let x = 0; x < 8; x++) {

		for(let y = 0; y < 8; y++) {
			if (y % 2 === 0) {square += `#`;}else {square += ` `;}
		}

	if (x % 2 !== 0) {square += `\n `;}else {square += `\n`;}

}

console.log(square);
```



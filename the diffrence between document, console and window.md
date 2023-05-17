2023-05-17

----
The browser make an html file when it reads `<!DOCTYPE html>`
- devide it into:
	- head
	- body
-

- !DOCTYPE html
	- html
		- head
			- metadata
		- body
			- elements

> this is the **DOM** -> Document Object Model

![[DOM.png]]

### Document
`document`
it is an object that controls in the html domument completely.

```js
document.querySelector('h1').style.color = "blue"
// this code selects the <h1> element and change it's color to blue.
```

```js
document.write('<h1>Hello</h1>')
// this code create a new h1 element
```


### console
`console`
it is a place in browser you can use it to try the any funciton without change the source code. 
it is an object you can use it to control in the browser console.
```js
console.log("Hello")
// this code print "Hello" in the console of browser
```

```js
console.error("helloe") 
// this code make an hello error in the console
```

### Window
`window`
it is an object controls in the browser generally.
```js
window.alert('hi')
//this code make an alert "hi"
```

```js
window.print()
//this code print the page  
```

window object has all the commands of js
window object is the **parent** of all objects

- window
	- document
	- console
> Window object is the parent


2023-05-28
[link](https://www.youtube.com/watch?v=CK2uHT45RC8&list=PLknwEmKsW8OuTqUDaFRBiAViDZ5uI3VcE&index=55)

----


### on click

```html
<button onclick="console.log('Hello!')">Click</button>
```


```js
function hello () {
	console.log("Hello!")
}
```
```html
<button onclick="hello()">Click</button>
```


```html
<button id="btn">Click</button>
```
```js
let btn = document.getElementById('btn');

btn.onclick = function hello () {
	console.log("Hello");
}
```


```html
<button id="btn">Click</button>
```
```js
let btn = document.getElementById('btn');

function hello () {
	console.log("Hello");
};

btn.onclick = hello;
```


### add event listener

```html
<button id="btn">Click</button>
```
```js
let btn = document.getElementById('btn');

btn.addEventListener('click', function () {
	console.log("Hello!");
})
```


### The difference between them - ChatGPT explaination:
||`onclick()`|`addEventListener()`|
|---|---|---|
|Syntax|Inline event handler assigned to HTML elements|Method used to attach event listeners to elements|
|Multiple Event Listeners|Only one event handler can be assigned|Multiple event listeners can be attached|
|Separation of Concerns|JavaScript code mixed with HTML markup|Promotes separation of JavaScript and HTML|
|Event Capture and Bubbling|Limited control over event capture and bubbling|Provides more control over event phases|


### google bard explaination:

The main difference between `addEventListener` and `onclick` is that `addEventListener` can attach multiple events to a single HTML element, whereas `onclick` can only associate the click event with a button. Moreover, `addEventListener` can only be utilized with the JavaScript code, and `onclick` event works in both HTML and JavaScript files.

Here is a table that summarizes the key differences between `addEventListener` and `onclick`:

|Feature|`addEventListener`|`onclick`|
|---|---|---|
|Can attach multiple events to a single element|Yes|No|
|Can only be used with JavaScript code|Yes|No|
|Can take a third argument to stop event propagation|Yes|No|
|Can be used in HTML attributes|No|Yes|

Here is an example of how to use `addEventListener` to attach multiple events to a single element:

Code snippet

```js
const element = document.getElementById("myButton");

element.addEventListener("click", function() {
  console.log("The button was clicked!");
});

element.addEventListener("mouseover", function() {
  console.log("The mouse is over the button!");
});
```

Here is an example of how to use `onclick` to associate the click event with a button:

Code snippet

```html
<button onclick="console.log('The button was clicked!')">Click me!</button>
```

As you can see, `addEventListener` is more flexible and powerful than `onclick`. It is the preferred way to attach event handlers to elements in JavaScript.



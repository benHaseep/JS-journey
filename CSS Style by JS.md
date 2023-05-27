2023-05-27

-----


```js
let container = document.getElementById("container");

container.innerText = "Hello World!"
// add text in the div.container.
```

First way to add CSS by JS.
the syntax: `element.style.property = "Value"`
```js
container.style.backgroundColor = "#444";

container.style.color = "#fa0";

container.style.padding = "10px";

container.style.borderLeft = "4px solid #fa0";
```

Second  way to add CSS by JS.
the syntax: `element.style.cssText = `` `
```js
container.style.cssText = `

background-color: #444;
color: #fa0;
padding: 10px;
border-left: 4px solid #fa0;

`
```

Third way to add CSS by JS.
the syntax: `element.style.setProperty("Property", "Value"`
```js
container.style.setProperty("color", "red", "important");
```

to remove property:
```js
container.style.removeProperty("color");
```

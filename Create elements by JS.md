2023-05-27

----

you can create full HTML page with JS.
```js
document.body.innerHTML = `

<h1>Hello, World!</h1>
<h3>Hello, World!</h3>
<p>Hello, World!</p>

`
```

```js
// ### Create Element:

let container = document.createElement("div");

let head = document.createElement("h1");

let img = document.createElement("img");

  

// ### Create Content for Elements:

let content = document.createTextNode("Hello, World!");

head.appendChild(content);

img.src = "/home/benhaseep/Pictures/benHaseep.jpeg";

img.style.width = "100px";

  

// ### Add childs to parent

container.appendChild(head);

container.appendChild(img);

document.body.appendChild(container);

container.style.backgroundColor = "#444";

container.style.textAlign = "center";

container.style.padding = "10px";
```
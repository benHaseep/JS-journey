2023-05-25

----
get - set - remove

```html
<body>

<img id="img" src="../Pictures/benHaseep.jpeg" alt="alt1" height="100" width="100">

</body> 
```
```js
let img = document.getElementById('img');

// ### Get
console.log(img); // <img id="img" src="../Pictures/benHaseep.jpeg" alt="alt1" width="100" height="100">
console.log(img.attributes); // class="image", id="img", src="../Pictures/benHaseep.jpeg", alt="alt1", width="100", height="100" ]
console.log(img.attributes[0]); // class="image"
console.log(img.alt); // alt1
console.log(img.src); // file:///home/benhaseep/Pictures/benHaseep.jpeg
console.log(img.className); // image
console.log(img.id); // img

  

// ### Modify
img.className = "test";
console.log(img.className); // test
// className modified

img.setAttribute("alt", "Ali");
console.log(img.alt);

  

// ### Set
img.title = "imgTitle";
console.log(img.title); // imgTitle

  

// ### Check
console.log(img.hasAttributes()); // true
console.log(img.hasAttribute("src")); // true
console.log(img.hasAttribute("asd")); // false

  

// ### Remove
img.removeAttribute('title');
console.log(img.title); // <empty string>
console.log(img.attributes); // [ class="test", id="img", src="../Pictures/benHaseep.jpeg", alt="Ali", width="100", height="100" ]
```



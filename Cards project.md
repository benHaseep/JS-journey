2023-05-27

-----

```js
let names = ["Ali", "Moaz", "Gabr"];
let ages = [18, 20, 15];


let container = document.createElement("div");
document.body.appendChild(container);
container.style.textAlign = "center";


function createCard (name='User', age='age') {
	// Create Elements
	let card = document.createElement("div");
	let title = document.createElement("h2");
	let ageP = document.createElement("p");
	let img = document.createElement("img");
	
	
	// Create Content
	let head = document.createTextNode(name);
	let agePContent = document.createTextNode(`${age} years old`);
	img.src = "https://placebear.com/100/100";
	
	
	// link elements with the parents
	title.appendChild(head);
	
	ageP.appendChild(agePContent);
	
	card.appendChild(title);
	card.appendChild(ageP);
	card.appendChild(img);
	
	container.appendChild(card);
	
	
	// Style
	card.style.width = "200px";
	card.style.padding = "10px"
	card.style.margin = "2px";
	card.style.backgroundColor = "#444";
	card.style.display = "inline-block";
	img.style.width = "100%";
};

for (let i = 0 ; i < 5 ; i++) {
	createCard(names[i], ages[i])
};
```


[The Result](https://codepen.io/benHaseep/pen/NWOmYqQ)

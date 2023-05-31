2023-05-30

----

The `sessionStorage` object let you store key/value pairs in the browser.

>The `sessionStorage` object stores data for only one session.
   (The data is deleted when the browser is closed).

-----------

- sessionStorage
	- setItem()
	- getItem()
	- key()
	- removeItem()
	- clear()
- Notes
	- new tab == new session
	- duplicate tab == copy session
	- new tab with the same URL == new session



### Set
```js
// Set

// There 3 ways to create item in session storage
window.sessionStorage.setItem('name', 'Haseep');
sessionStorage.name = 'Haseep';
sessionStorage['name'] = 'Haseep';
// 'name' is the key, 'Haseep' is the value
```


### Get
Get the values
```js
window.sessionStorage.setItem('name', 'Haseep');
sessionStorage.name = 'Haseep';
sessionStorage['name'] = 'Haseep';


// Get

// There are 3 ways to get items from session storage:
console.log(sessionStorage.getItem('name')); // Haseep
console.log(sessionStorage.name); // Haseep
console.log(sessionStorage['name']); // Haseep
```

Get the keys
```js
console.log(sessionStorage.key(0)); // name
// key takes the index and give you the key.
```

### Remove

```js
// remove one item:
sessionStorage.removeItem('name');

// remove all date:
sessionStorage.clear();
```


[[Session storage]]
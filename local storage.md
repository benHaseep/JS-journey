2023-05-29

----


The `localStorage` object allows you to save key/value pairs in the browser.

> The localStorage object stores data with no expiration date.
> The data is not deleted when the browser is closed, and are available for future sessions.

- localStorage
	- setItem()
	- getItem()
	- key()
	- removeItem()
	- clear()
- Notes
	- No expiration time
	- http & https
	- private tab


### Set
```js
// Set

// There 3 ways to create item in local storage
window.localStorage.setItem('name', 'Haseep');
localStorage.name = 'Haseep';
localStorage['name'] = 'Haseep';
// 'name' is the key, 'Haseep' is the value
```


### Get
Get the values
```js
window.localStorage.setItem('name', 'Haseep');
localStorage.name = 'Haseep';
localStorage['name'] = 'Haseep';


// Get

// There are 3 ways to get items from local storage:
console.log(localStorage.getItem('name')); // Haseep
console.log(localStorage.name); // Haseep
console.log(localStorage['name']); // Haseep
```

Get the keys
```js
console.log(localStorage.key(0)); // name
// key takes the index and give you the key.
```

### Remove

```js
// remove one item:
localStorage.removeItem('name');

// remove all date:
localStorage.clear();
```


[[Session storage]]
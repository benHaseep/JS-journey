2023-06-10

-----

JSON.parse      -->  Convert text data to JS object.
JSON.stringify  -->  Convert JS object to JSON.

JSON is a text format

```js
const myJsonObjectFromServer = '{"name": "Haseep", "age":21}';

console.log(myJsonObjectFromServer); // {"name": "Haseep", "age":21}

console.log(typeof myJsonObjectFromServer); // string

  

const myJsObject = JSON.parse(myJsonObjectFromServer);

console.log(myJsObject); // Object { name: "Haseep", age: 21 }

console.log(typeof myJsObject); // object

  

myJsObject["name"] = "benHaseep";


const myJsonObjectToServer = JSON.stringify(myJsObject);

console.log(myJsonObjectToServer); // {"name":"benHaseep","age":21}

console.log(typeof myJsonObjectToServer); // string
```


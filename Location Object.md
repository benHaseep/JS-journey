2023-05-29

----

### URL
// https://twitter.com/benHaseep == href -> hypertext reference

// https: == protocol
// twitter.com == host name
// /benHaseep/ == path name

### Location Object
the object that deal with URLS.

```js
console.log(location); // file:///home/benhaseep/Code/test.html
console.log(location.protocol); // file:
console.log(location.pathname); // /home/benhaseep/Code/test.html

// you can change the values of these objects
location.hostname = 'twitter.com'  // redirect you to twitter

```

```js
location.assign('https://www.twitter.com'); // redirect you to twitter
// assign: you can back to previous page
location.replace('https://www.twitter.com'); // redirect you to twitter
// replace: you can't back to the previous page
```


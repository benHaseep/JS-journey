2023-05-29

-----

## The Window Screen Object
The screen object contains information about the visitor's screen.

```js
console.log(window.screen);

// Screen { availWidth: 1366, availHeight: 736, width: 1366, height: 768, colorDepth: 24, pixelDepth: 24, top: 0, left: 0, availTop: 32, availLeft: 0 }

console.log(typeof screen); // object

console.log(screen.width); // 1366
console.log(screen.height); // 768

console.log(screen.availWidth); // 1366
console.log(screen.availHeight); // 736

console.log(screen.colorDepth); // 24
console.log(screen.pixelDepth); // 24

console.log(screen.orientation.type); // landscape-primary
```


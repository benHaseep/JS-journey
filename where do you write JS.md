
2023-05-17

-----

### 1.**You can writ JS code in html head or body** 

``` html
<html> 
	<head>
		<script><document.write("hello from js")/script>
	</head>
	
	<body>
		<script><document.write("hello from js")/script>
	</body>
</html>
```

``` js
document.write("hello from js")
// this code is adding text to html document
```

### 2. You can write JS code in external file
- create a file with `.js` extention.
- link this file with HTML document:
	- `<script src='path of js file'> </script>`


### notes
[[Linking JS wiht HTML document notes]]
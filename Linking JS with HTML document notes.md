2023-05-17

------

The compiler reads the code in the html document from top to bottom line by line, so take care when linking js with html document.

``` JavaScript
document.querySelector('h1').style.color = 'red';
// If you put the script code in the head or linked the js file in the head, iIt probably won't work. because the compiler reads the html document line by line and in this case you are trying to change <h1> before the compiler read it.
```

- You can put the script code in at the end of the body To ensure that it works.
- You can use onload in the js file if you want to run the code after html document loaded to ensure that it work.


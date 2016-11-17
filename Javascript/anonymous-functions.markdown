# Anonymous functions 

If you use a **function expression** to define a function's name. The syntax is: 

```javascript 
function [name]([p1[, p2[, ...]]]) {
	//statements
}
```

An example of an **anonymous** function: 

```javascript
var square = function(x) {
	return x * x;
}; 
```

The downsides to anonymous function expressions are: 

* You are unable to refer to the function within itself e.g. for recursion.

* You can't debug easily, especially in minified code. 

* You can lose the clarity gained by a **function declaration**. 

From [**Enki**](https://www.enki.com/)
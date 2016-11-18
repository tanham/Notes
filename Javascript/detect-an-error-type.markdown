# Detect an error type 

Using the `try/catch` block you can catch an exception then figure out what type of error occured in your code. For example: 

```javascript
try {
	eval('5 + / 3');
}
catch(e) {
	if(e.constructor == SyntaxError) {
		// handle if is SyntaxError
	}
	console.log(e.constructor.name);
}
```

The code snippet above will try to run `eval('5 + / 3');` which is a `SyntaxError`. 

You can get the name of the error with `e.constructor.name`.

In addition, if you think you can handle a specific exception, checking for it is easy: `e.constructor == SyntaxError`. 
 
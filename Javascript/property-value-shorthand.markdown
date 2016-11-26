# Property Value Shorthand 

It is very common to return an object frim a function with a property the same name as a source value declard elsewhere e.g.

```javascript 
function test(){
	var name = "Enki"; 

	return {
		name: name
	}
}
```

ES6 provides a convenient shortcut to do this that allows you to drop the proprty name if you want it to be the same as the source variable: 

```javascript 
function test(){
	var name = "enki";

	return{
		name
	};
}

test(); //{ name: "enki" }
```

Note an exception will be thrown at run time if you specify a value that doesn't exist in your return object. 

Source: [**Enki**](https://www.enki.com/)
# Function call method 

The `call` method allows changing the this object of a function from the original context to the context of the new object specified by `thisObj`. 

`currObj` is the object to be used as the current object. 

`arg1`, `arg2`, ... , `argN` are arguements passed onto the method. 

If `currObj` is not supplied, the `currObj` is set to the global object. 

Creating a function to call returning a string of the object and arguments: 

```javascript
function callObject(arg1, arg2) {
	var str; 
	str += "Object: " + this + ". ";
	str += "Arguements: "
	for (i in callObject.arguments){
		str += callObject.arguments[i] + " ";
	}
	return str; 
}  
```

Calling the function using the call method: 

```javascript
callObject.call(2, 4, 6);
```

The current object would be changed to 2, and the string generated and returned would be: 

```javascript
str = "Object: 2. Arguements: 4 6 "
```



From [**Enki**](https://www.enki.com/)



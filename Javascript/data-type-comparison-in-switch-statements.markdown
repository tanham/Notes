# Data type comparison in switch statements

The `==` operator does not care for types. Therefore the following alert will show: 

```javascript
var test = 5; 
if(test == '5'){
	alert("Hello World");
}
```

However, Javascript is using strict comparision (similar to `===`) in `switch` statements: 

````javascript
var test = 5;
switch(test){
	case '5':
	alert("Hello World");
}
```

This alert will not show since the data types do not match. 

From [**Enki**](https://www.enki.com/)
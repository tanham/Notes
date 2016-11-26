# Default Params 

In Ecmascript if a function with parameters is called without supplying arguements then any arguements are undefined: 

```javascript 
function test(x){
	console.log(x); //undefined
}

test();
```

If this is a valid use case for the function the developers would test to see if arguement were intialized or ise truthy/falsy shortcuts to set intial values: 

```javascript
function test(x,y){
	if(x==undefined){
		x=1; //default 
	}
	y = y || "default"; 

	console.log(x); //1
	console.log(y); //"default"
} 
```

Default parameters allow you to declare a default to be used if an arguement is not supplied. 

To declare a default parameter simply specify the default value next to the arguement in the function signature: 

```javascript
function test(x=1, y="default"){
	...
}
```

Default parameters can also be a function or even other parameters: 

```javascript 
function test(x=someFunction()){
	...
}

function test(x="1", y=x){
	...
}
```

Default parameters are a great easy to use feature that will result in more succinct and readable code. 

Source: [**Enki**](https://www.enki.com/)
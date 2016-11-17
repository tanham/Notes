# Catch is block scoped 

The `catch` clause of a `try...catch` statement is **block** scoped. This is different to the rest of Javascript which is **function** scoped. 

```javascript 
try {
	//..
}  
catch (err) {
	// err is block scoped
}
```

Many linters fail to recognize that it is valid to have mulitiple `try...catch` statements in the same scope, all using `err`, without it being a repeated variable declaration. 

from [**Enki**](https://www.enki.com/) 
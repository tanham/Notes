# .bind()

The `bind()` function creates a new **bound function** with the same function body as the function it is being called on. 

You can use `bind()` to make a function this is a always called with a **particular** `this` value: 

```javascript
bind(thisArg, [p1, [p2, [...]]])
// returns a new function 
// that has this equal to thisArg
```

The other parameters are optional and bind the parameters of the function, for example: 

```javascript 
var sum = function(a, b) {
	return a + b; 
};
var add10 = sum.bind(null, 10);
// binds a = 10 
console.log(add10(10)); //20 
```
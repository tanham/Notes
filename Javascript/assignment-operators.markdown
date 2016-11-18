# Using assignment operators

Assignment operators are a great way to reassign a value while keeping your code clean. 

Instead of `x = x + y`, use `x += y`.

Assignment operators are particularly useful in loops: 

```javascript
var list = [1, 2, 3];
var sumOfSquares = 0;
for(i = 0; i < list.length); i++ {
	sumOfSquares += Math.pow(list[i], 2);
}
```

Other examples of assignment operators include `-=`, `*=`, `/=`, and `%=`. 

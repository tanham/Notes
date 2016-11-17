# Use the apply function to get the min or max of an array

Common idiom: 

```javascript 
var nums = [1, 3, 2]
Math.max.apply(Math,nums) // 3 
Math.min.apply(Math,nums) //1
```

Note that `apply` is required here because `Math.max` does not directly support arrays as an arguement. 

More examples: 

```javascript
Math.max(1, 3, 2) // 3 
Math.max([1, 3, 2]) // NaN
Math.max.apply([1, 3, 2]) // -Infinity 
Math.max.apply({}, [1, 3, 2]) // 3
Math.max.apply(null, [1, 3, 2]) // 3
Math.max.apply(Math, [1, 3, 2]) // 3
```

The first arguement provided to `.apply` is the "context". The value of this context does not matter is this case, but it is common practice when using `.apply` to provide the relevant class as context.

From [**Enki**](https://www.enki.com/) 
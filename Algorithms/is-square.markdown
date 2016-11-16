# isSquare 

Given an integral number, determine if it's a square number:

###Examples:
```
isSquare(-1) // => false
isSquare( 3) // => false
isSquare( 4) // => true
isSquare(25) // => true
isSquare(26) // => false
```

### My solution:

```javascript
var isSquare = function(n){
  var squareRoot = Math.sqrt(n);
  if(squareRoot % 1 === 0 ){
    return true;
  } else
    return false; 
  }
```

### Best Solution (on codewars):

```javascript
function isSquare(n) {
  return Math.sqrt(n) % 1 === 0;
}
```

### reference: 

[`Math.sqrt()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/sqrt)
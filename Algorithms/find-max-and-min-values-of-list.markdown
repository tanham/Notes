# Find Maximum and Minimum Values of a List

Write two functions, max and min (maximum and minimum in PHP) that take a(n) array/vector of integers list as input and outputs, respectively, the largest and lowest number in that array/vector.

### Examples

`max([4,6,2,1,9,63,-134,566]) returns 566`
`min([-52, 56, 30, 29, -54, 0, -110]) returns -110`
`max([5]) returns 5`
`min([42, 54, 65, 87, 0]) returns 0`

### My solution:

```javascript
var min = function(list){
    
    return Math.min.apply(null, list);
}

var max = function(list){
    
    return Math.max.apply(null, list);
}
```javascript
const min = (list) => Math.min(...list);
const max = (list) => Math.max(...list);
```

### Best Solution (on codewars):

### references: 

[`Math.max()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/min)

[`Math.min()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Math/max)

[`.apply()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Function/apply)
# Descending Order

Write a function that can take any non-negative integer as a argument and return it with it's digits in descending order. Descending order means that you take the highest digit and place the next highest digit immediately after it.

###Examples:

Input: `145263` Output: `654321`

Input: `1254859723` Output: `9875543221`

### My solution: 

```javascript
function descendingOrder(num){
  return parseInt(num.toString().split("").sort().reverse().join(""), 10);
}
```

### Best soulation (on codewars): 

```javascript 
function descendingOrder(n){
  return parseInt(String(n).split('').sort().reverse().join(''))
}
```

### references

[`parseInt()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/parseInt)
[`.sort()`](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects/Array/sort)
[`.reverse()`](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects/Array/reverse)
[`.toString()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Object/toString)
[`.join()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/join)
[`.split()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/split)


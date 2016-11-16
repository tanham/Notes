# Recursive reverse string

Your objective is to complete a recursive function reverse() that receives str as String and returns the same string in reverse order

Rules:

* reverse function should be executed only N times. N = length of the input string
* helper functions are not allowed
* changing the signature of the function is not allowed

###Examples:

```
reverse("hello world") = "dlrow olleh" (N = 11)
reverse("abcd") = "dcba" (N = 4)
reverse("12345") = "54321" (N = 5)
```

### My solution:

```javascript
function reverse(str) {
  if(str.length <= 1) return str;
  else {
  return reverse(str.substring(1)) + str.charAt(0);
  } 
}
```

### Best Solution (on codewars):

```javascript
function reverse(str) {
    return str.length > 1 ? reverse(str.slice(1)) + str[0] : str;
}
```

### references: 

[recursion](https://developer.mozilla.org/en-US/docs/Glossary/Recursion)
[`.reverse()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/reverse)
[`.charAt()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/charAt)
[`str.substring()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/substring)
[`.slice()`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/slice)
# Vowel Count 

Return the number (count) of vowels in the given string.

We will consider a, e, i, o, and u as vowels for this Kata.

### My solution:

```javascript
function getCount(str) {
    var m = str.match(/[aeiou]/gi);
    
    if(m == null) {
      return 0;
    } else {
      return m.length;
  }
}
```

### Best solution: 

```javascript
function getCount(str) {
  return (str.match(/[aeiou]/ig)||[]).length;
}
```

### references: 

[`String.prototype.match()`](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects/String/match)

[`RegExp`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/RegExp)


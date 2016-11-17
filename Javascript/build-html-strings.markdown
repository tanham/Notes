# Most efficient way to build HTML strings 

On modern browers, building `HTML` strings with `.join()` is less efficient than the naive method.

So, adding the values to an array and then joining them at the end: 

```javascript
var html = [];
for(var i = 0; i < 100; i++) {
	html.push('<p>', i, '</p>');
}
html = html.join('');
```

Runs slower than the naive method of building `HTML` strings using `+=`: 

```javascript
var html = '';
for(var i = 0; i < 100; i++) {
	html += '<p>' + i + '</p>'
}
```


[**Enki**](https://www.enki.com/)
# String Extensions 

ES6 expands on existing primitives to fix some long time issues and add useful functionality. 

In previous versions of EcmaScrit if you wanted to use Unicode characters one method was to use *String.fromCharCode*: 

```javascript 
String.fromCharCode(65); //A
```

However *fromCharCode* doesn't work with all possible unicode values. 

ES^ introduces a new method *fromCodePoint* that can be used to work with all unicode values up to 21 bits: 

```javascript 
String.fromCodePoint(65); //A
String.fromCodePoint(65,66,67); //ABC
```

Source: [Enki App](https://enki.com)
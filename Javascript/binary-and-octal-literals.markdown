# Binary and Octal Literals 

EcmaScript 6 introduces the ability to declare binary and octal literals. 

Previously if you wanted to work with binary or octal numbers you would use the *parseInt* function and specify the *base* or *radix* you were working with. 

For example binary numbers the base is 2 and for octal 8: 

```javascript 
console.log(parseInt("101", 2)); //5
console.log(parseInt("11",8)); //9
```

With ES6 we can use the *0b* prefix to declare a binary number: 

```javascript
console.log(0b101); //5
``

Octal numbers can be declared with *0o*:

```javascript
console.log(0o11); //9
```

Source: [Enki App](https://enki.com)
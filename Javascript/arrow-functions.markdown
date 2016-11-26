# Arrows Functions 

Arrow functions (aka lambda functions) provide a short hand syntax to declare functions expressions and can save some tedious code around EcmaScript's *this* keyword. 

The arrow function (or "fat arrow") has two parts placed either side of => e.g.

```javascript 
(optional) inputs => expression
```

On the left hand side are the arguements (which are optional) and the right hand side contains the expression itself.

Below we use arrow function syntax to declare a function that accepts two parameters (x and y) and will add them together: 

```javascript 
var add = (x,y) => x+y
add(2,4); //6
```

**Shortening arrow functions**

If a function has no arguements you can shorten it to: 

```javascript
var doubleInput = x => x*2;
```

When using *arrow functions* and more complex expressions you must enclose the expression with curly brackets: 

```javascript 
var func = 
x => {x++; return x * 2; }
```

If you want to return an object then be sure to ensure the return is wrapped in brackets so the inerpreter knows how to process the code: 

```javascript 
var obj = () =>
({firstname: "John", lastname: "Smith"});
```

Arrows functions work particularly well when used with methods such as map & filter as allow you to succinctly declare you intention:

```javascript 
var firstNames = 
people.map(p => p.firstname); 
```
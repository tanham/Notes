# Number Extensions

Number benefits from a number of new methods saving you from writing your own potentially error prone implementaiton.

There are a large number so here are some of the ones that are likely to have more use: 

**Number.isFinite**

Determines whethera number is finite (finite means that it could be measured or have a value). 

```javascript
Number.isFinite(Infinity); //false
Number.isFinite(100); //true
```

**Number.isInteger**

Determines if a number is an integer or not. 

```javacript 
Number.isInteger(1); // true 
Number.isInteger(0.1); //false
```

**Number.isNaN**

Before ES6 it was difficult to test if a value was equal to *NaN*. This is because NaN == NaN evaluates to false. 

Whilst a global *isNaN* function has existed in previous versions it has the issue that it converts values which makes it hard to test if something is really *NaN*: 

```javascipt 
isNan("Enki")==true; //true
```

Number.isNaN allows you to easily test if a number really is NaN: 

```javascript 
Number.isNaN(1); //false
Number.isNaN(Number.NaN); //true
```

**Number.EPSILON**

Number.EPSILON is the smallest value less than 1 that can be represented as a number and is intended for advanced uses such as testing equality: 

```javascript
Number.EPSILON;
//2.220446049250313e-16
```

**Number.isSafeIntegar**

```javascript
Number.isSafeIntegar(3); //true
var unsafe = Math.pow(2, 53);
Number.isSafeIntegar(unsafe); //false
```


Source: [Enki App](https://enki.com)
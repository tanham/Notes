### Math 


#### Math.floor

returns the largest integer less than or equal to a given number

```Math.floor( 45.95); //  45```
```Math.floor( 45.05); //  45```
```Math.floor(  4   ); //   4```
```Math.floor(-45.05); // -46```
```Math.floor(-45.95); // -46```

#### Math.ceil 

returns the smallest integer greater than or equal to a given number

```Math.ceil(4);      // 4```
```Math.ceil(7.004);  // 8```
```Math.ceil(-0.95);  // -0```
```Math.ceil(-4);     // -4```
```Math.ceil(-7.004); // -7```

#### Math.round

returns the value of a number rounded to the nearest integer

```Math.round( 20.49); //  20```
```Math.round( 20.5);  //  21```
```Math.round( 42  );  //  42```
```Math.round(-20.5);  // -20```
```Math.round(-20.51); // -21```


#### Math.random

generate random integer between 0 and 1

```function randomNumber() {
	return Math.round();
}```

#### Example

Math.max & Math.Min

```function sumAll(arr) {
  var max = Math.max(arr[0], arr[1]);
  var min = Math.min(arr[0], arr[1]);
  var temp = 0;```
  
  ```for(var i = min; i <= max; i++){
    temp += i;
  }```
  ```return temp; ```
}```
sumAll([1, 4]);```


[Read more - MDN](https://developer.mozilla.org/en/docs/Web/JavaScript/Reference/Global_Objects/Math)
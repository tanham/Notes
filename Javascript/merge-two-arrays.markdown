# How to merge two arrays

`concat` is not always the best approach to merging arrays as it generates a new array. 

Since `var`s are passed by reference, `concat` may mess up a reference.

Instead: 

```javascript 
var array1 = [1, 2, 3];
var array2 = [4, 5, 6]; 
```

Merge them, adding the second one after the first one: 

```javascript 
Array.prototype.push.apply(array1, array2); 
```  
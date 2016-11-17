# Difference between **.call** and **.apply** methods 

The main difference between the two methods is the way they handle arguements. 

`.call` methods requires explicit parameters while `.apply` lets you invoke the method using an array as arguement. 

**Example** 

```javascript 
function.call(obj, 1, 2, 3);
function.apply(obj, [1, 2, 3]); 
```

From [**Enki**](https://www.enki.com/)
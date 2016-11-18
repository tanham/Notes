# Use splice() to remove an item from an array 

Use `splice` instead of using `delete` to erase an item from an array. Using `delete` replaces the iten with `undefined` instead of removing it from the array entirely. 

Instead of: 

```javascript 
var items = [12, 548, 'a', 2];
items.length; // returns 4
delete.items[3]; // returns true
items.length; // returns 4
//items = [12, 548, 'a', undefined x 1]
```

Use: 
```javascript
var items = [12, 548, 'a', 2];
items.length; // returns 4
items.splice(3,1); 
items.length; // returns 3
//items = [12, 548, 'a']
```

The delete method should only be used to delete an object property. 

From [**Enki**](https://www.enki.com/)
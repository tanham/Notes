# Detect online connection 

Check if a user is connected to internet with the help of `navigator` property. 

```javascript 
if(navigator.onLine) {
	//..
}
```

This will return a `Boolean` value for whether or not the user is connected to the internet.

The `offline` and `online` events can also be used with a listener. 

```javascript
window.addEventListener('online', myFunction);
window.addEventListener('offline', myFunction);
```
from **Enki**
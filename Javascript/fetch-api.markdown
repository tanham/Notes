# Fetch API 

The *Fetch API* provides an interface to fetch resources from across a network. 

The `fetch()` method is used for making requests and fetching resources. It takes one compulsory argument - the path to the resource you want to fetch. 

It returns a promise that resolves to the response to that request, whethr it's successful or not. 

It provides a more powerful and flexible interface than `XMLHttpRequest`.

Example of fetch response handling: 

```javascript
var myHeaders = new Headers();

var myOptions = { method: 'GET',
				  headers: myHeaders,
				  mode: 'cors',
				  cache: 'default' };

fetch('/the/url', myOptions)
	.then(function(response) {
		return // ...
	}).then(function(returnValue) {
		// ...
	}).catch(function(error) {
		console.log("Problem occured: " + error.message);
	});
```

From [**Enki**](https://www.enki.com/)
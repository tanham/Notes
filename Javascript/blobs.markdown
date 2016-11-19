# Blobs 

A *blob* object represents an "almost file" object of raw data. It represents data that      isn't in JavaScript's standard format. You use *FileReader* to read data from a blob. 

To create a blob, use the bblob constructor: 

```javascipt
var debug = {hello: "world"};
var blob = ne Blob([
	JSON.stringify(debug, null, 2)
	], {type : 'application/json'});
```

TO create a subset of a blob, use the slice() method: 

```javascript 
var blob = instanceOfBlob.slice([
	start [, eend [, contentType]]
	]); 
```

From [**Enki**](https://www.enki.com/)
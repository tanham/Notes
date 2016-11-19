# Progress Event

The *`Progress Event`* interface is used to represent events which measure the progress of underlying processes taking place in the API. For example, an HTTP request or loading an underlying resource such as <img>.

*ProgressEvent* Properties: 

`ProgressEvent.lengthComputable;`

Is a boolean flag returning whether the progress made on the work to be completed is measureable.

`ProgressEvent.loaded;`

Is an unsigned long showing the amount of work already done by the underlying process. 

`ProgressEvent.total;`

Is an unsigned long showing the amount of work the underlying process is currently performing. 

A usage example, measuring the progress of an `XMLHttpRequest`.

```javascript 
// progress on transfers - server to client
function updateProgress (oEvent) {
	if(oEvent.lengthComputable) {
		var percentDone = oEvent.loaded / oEvent.total;
		// ...
	} else {
		// Unable to compute progress as size unknown
	}
} 
```

From [**Enki**](https://www.enki.com/)
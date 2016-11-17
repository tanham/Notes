# Getting the real dimensions of an image

Find original dimensions of an image via `natural` properties: 

```javascript
this.naturalWidth;
this.naturalHeight;
```

Keep in mind that these properties are read-only. An `img`'s `onload()` event must be loaded first as you can't check the dimensions prior to loading it. 

```javascript 
myImg.addEventListener('load', function() {
	console.log('Width: ', this.naturalWidth);
	console.log('Height: ', this.naturalHeight);

});
```

This same result can be acheived by defining the `.onload` property of an image:

```javascript 
myImg.onload = function() {
	console.log('Width: ', this.naturalWidth);
	console.log('Height: ', this.naturalHeight);		
}
```

From [**Enki**](https://www.enki.com/)
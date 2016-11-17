# Prevent background image flicker in IE

**Internet Explorer** proved to have problems when loading cached background images as a flicker effect commonly appear. 

A quick fix is a adding this **JS** script: 

```javascript
<script type="text/javascript">
try {
document.execCommand
	('BackgroundImageCache', false, true);
}
catch(e) {};
</script>
```

However, on **IE 10** this won't solve the problem. This version of the browser won't load cached images via **CSS**. As to solve this you need to force load the image: 

```javascript
background-image: url('background1.jpg')
```

In **HTML**:

```html 
<img src='background1.jpg'
style='display:none' />
```

from [**Enki**](https://www.enki.com/)
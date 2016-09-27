### Display 

* `display` - every element has a default `display. The default for most elements is usually `block` or `inline`. A block element is often called a block-level element. An inline element is always just called an inline element.
	
	* `block` - `div` is the standard block-level element. A block-level element starts on a new line and stretches out to the left and right as far as it can. Other common block-level elements are p and form, and new in HTML5 are header, footer, section, and more.
	
	* `inline` - `span` is the standard inline element. An inline element can wrap some text inside a paragraph `<span> like this </span>` without disrupting the flow of that paragraph. The a element is the most common inline element, since you use them for links.


	* `none` - Setting display to none will render the page as though the element does not exist.

	* other
		see https://developer.mozilla.org/en-US/docs/Web/CSS/display 



### Horizantal Center 

* Set width of block level element and then set margin to `auto` to horizantally center. The element will take up the width you specify, then the remaining space will be split evenly between the two margins.

* use max-width for responsive design.



### Box-sizing 

* the block of code below will prevent the elements stretching border and padding beyond width: 

```* {
  -webkit-box-sizing: border-box;
     -moz-box-sizing: border-box;
          box-sizing: border-box;
} ```

### position 
see position example [here](http://learnlayout.com/position-example.html).

* static - The default value. An element with position: static; is not positioned in any special way. A static element is said to be not positioned and an element with its position set to anything else is said to be positioned.

```
.static {
  position: static;
}
```
* relative - behaves the same as static unless you add extra properties 
	
	* Setting the `top`, `right`, `bottom`, and `left` properties of a relatively-positioned element will cause it to be adjusted away from its normal position. Other content will not be adjusted to fit into any gap left by the element.

```.relative1 {
  position: relative;
}
.relative2 {
  position: relative;
  top: -20px;
  left: 20px;
  background-color: white;
  width: 500px;
}```


* fixed - positioned relative to the viewport - which means it stays in the same place even if the page is scrolled. As with relative, the top, right, bottom, and left properties are used.

```.fixed {
  position: fixed;
  bottom: 0;
  right: 0;
  width: 200px;
  background-color: white;
}```

* absolute - behaves like fixed except relative to the nearest positioned ancestor instead of relative to the viewport.

```
.relative {
  position: relative;
  width: 600px;
  height: 400px;
}
.absolute {
  position: absolute;
  top: 120px;
  right: 0;
  width: 300px;
  height: 200px;
}
``` 



source http://learnlayout.com/
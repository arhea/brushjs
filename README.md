# BrushJS
BrushJS provides a single API for drawing on the canvas as well as writing to SVG.

## Example

```html
<canvas id="SVG" width="600" height="600" style="border: solid 1px #999999; float: left;">Your browser does not support canvas.</canvas>
<div id="xml" style="border: solid 1px #999999; float: left;"></div>
```

```javascript
var ctx = new Brush( "#SVG" );
ctx.fillStyle = "#333333";
ctx.font = "20px sans-serif";
ctx.fillText( "Sample Text" , 300 , 300 );

document.getElementById( "xml" ).innerHTML = ctx.toDataURL( "image/svg+xml" );
```

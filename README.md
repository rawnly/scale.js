# Scale.js
## Include
-----
Download the file and include `scale.js` in your document after including jQuery.
```html
	<!-- Your <head> -->
	<script src="https://ajax.googleapis.com/ajax/libs/jquery/1.11.0/jquery.min.js"></script>

	<script src="https://cdn.rawgit.com/Rawnly/scale.js/master/dist/js/scale.js" > </script>
```
## Usage
--------
### Via data attributes
To easily scale an element, add `data-scale` to the element you want to use, and specify a scale factor ( see the example below), then you can also specify a unit for responsive text  ( like `vh` or `vh` or something else ) by adding `data-unit` to the same element.

**Syntax:**
```html
<p data-scale="$factor" data-unit="$unit" style=" font-size='10px' "> Sample </p>
<!-- Text size will be -->
<!-- 10 x $factor = $result $unit -->
```

**Example:**

```html
<p data-scale="0.2" data-unit="vw" style=" font-size='10px' "> Hello World </p>
<!-- Text size will be -->
<!-- 10 x 0.2 = 2vw -->
```

### Via Javascript
To call the scale plugin manually, simply select your target element with **jQuery** and do the following:
```javascript
	$("selector").scale( factor, { u: 'unit' } );
```
**Example:**
```javascript
    $('selector').scale( 1, { u: 'px' } );
```
# Note:

* To make a text responsive you need to scale it via JavaScript, in case don't worry about console who alerts you about there aren't targets with `data-scale` / `data-unit` attributes.

* Please report bugs via [mail](mailto:rawnlydev@gmail.com) or open an issue here on GitHub.

# Changelog
* [ 12/09/2016 ] **v0.1.0** - Scale.js was born!

# LICENSE
#### The MIT License (MIT)
##### Copyright © 2016 <a href="http://github.com/Rawnly/"> Federico Vitale </a>
Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation <br>
files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, <br>
modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the <br>
Software is furnished to do so, subject to the following conditions:
The above copyright notice and this permission notice shall be included in all copies or substantial portions of the
Software.<br>

**
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE
WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE,
ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
**

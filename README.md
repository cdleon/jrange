JRange
================

Simple-slider.js is a lightweight pure javascript slider. 

  - Vertical and Horizontal orientations
  - Pure Javascript, no dependencies
  - Supports touch motion
  - Easy very flexible css styling

### Version
1.0.0

### Installation

Simply include simple-slider.js at the end of your project, just before the closing body tag.

```html
...
<script type="text/javascript" src="js/cdlm-slider.js"></script>
</body>
```

### Usage

Instantiate the simple_slider class and add the config parameters

*  **_@param_** (_string_)**targ** - Element target where the slider is to be installed. Use  **.** or **#** to target class or id identifier respectively (_class target installs on first ocurrence of class element_).  
*  **_@param_** (_int_)**max_val** - Slider max
*  **_@param_** (_int_)**init_val** - Value where slider starts
*  **_@param_** (_string_)**write_to** - (_option_) write slider current value onto (_hereby_) specified element
*  **_@param_** (_bool_)**verbose** - (_option_) true to output slider current value to console log.
*  **_@param_** (_string_)**orient** - _"vertical"_ or _"horizontal"_ for vertical or horizontal slider mode. **NOTE:** match css styling to cohere with mode see **_styling_**.

```html
...
<script type="text/javascript" src="js/cdlm-slider.js"></script>
<script type="text/javascript">
	var vsl = new cdlm_slider({	
								targ: '#any-div',
								max_val: 500,
								init_val: 0,
								write_to: '#any-div',
								verbose: false,
								orient: 'vertical'
							});
</script>
</body>
```


### Styling

Simple Slider adapts to pretty much any css styling. NOTE: style widths and heights coherently to match slider vertical and horizontal modes: Use larger track height than track width for vertical mode, and larger track width that track height for horizontal mode.

Stylable components:

* **_#cdlm-slider-track_** - Track space for slider thumb
* **_#cdlm-slider-track-upper_** - Element div representing value of slider, increases and decreases with value on top of thumb (only in supported in vertical mode)
* **_#cdlm-slider-track-lower_** - Not supported yet
* **_#cdlm-slider-thumb_** - Thumb of the slider


### Development

Ask for pull requests!


### Todo's

 - Refactor slider class
 - Add lower track styling support
 - Force relative position for thumb, so always clickable
 - Add left and right track styling support for horizontal mode
 - Add height/width proportion check to trigger error when css style does not match slider mode

License
----

MIT


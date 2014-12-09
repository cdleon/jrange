simple-slider.js
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

* **_@param_** (_string_)**targ** - Element target where the slider is to be installed. Use  **.** or **#** to target class or id identifier respectively (_class target installs on first ocurrence of class element_).  
* ** _@param_** (_int_)**max_val** - Slider max
*  **_@param_** (_int_)**init_val** - Value where slider starts
*  **_@param_** (_string_)**write_to** - (_option_) write slider current value onto (_hereby_) specified element
*  **_@param_** (_bool_)**verbose** - (_option_) true to output slider current value to console log.
*  **_@param_** (_string_)**orient** - _"vertical"_ or _"horizontal"_ for vertical or horizontal slider mode. **NOTE:** match css styling to cohere with mode see **_styling_**.

```html
...
<script type="text/javascript" src="js/cdlm-slider.js"></script>
<script type="text/javascript">
	var vsl = new cdlm_slider({	
								targ: '.test',
								max_val: 500,
								init_val: 0,
								write_to: '#cdlm-slider-thumb',
								verbose: false,
								orient: 'vertical'
							});
</script>
</body>
```


### Styling

Simple Slider adapts to pretty much any css styling. NOTE: style widths and heights coherently to match slider vertical and horizontal modes: Use larger track height than track width for vertical mode, and larger track width that track height for horizontal mode.

Stylable elements:


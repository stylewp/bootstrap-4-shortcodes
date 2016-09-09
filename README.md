Bootstrap 4 Shortcodes for WordPress
===

![WordPress Rating](https://img.shields.io/wordpress/plugin/r/bootstrap-4-shortcodes.svg) ![WordPress Downloads](https://img.shields.io/wordpress/plugin/dt/bootstrap-4-shortcodes.svg)

WordPress plugin that provides shortcodes for easier use of the Bootstrap 4 styles and components in your content.

**Bootstrap 4 Shortcodes for WordPress** creates a simple, out of the way button just above the WordPress TinyMCE editor (next to the "Add Media" button) which pops up the plugin's documentation and shortcode examples for reference and handy "Insert Example" links to send the example shortcodes straight to the editor. There are no additional TinyMCE buttons to clutter up your screen, just great, easy to use shortcodes!

## Requirements
![Tested in WordPress](https://img.shields.io/wordpress/v/bootstrap-4-shortcodes.svg) ![PHP 5.3+](https://img.shields.io/badge/PHP-5.3%2B-blue.svg) ![Bootstrap](https://img.shields.io/badge/Bootstrap-4-6f5499.svg)

This plugin won't do anything if you don't have WordPress theme built with the [Bootstrap 4](http://getbootstrap.com/) framework. **This plugin does not include the Bootstrap framework**.

The plugin is tested to work with ```Bootstrap 4``` and ```WordPress 4.6``` and **requires PHP 5.3 or later**.

## Shortcode Reference

### Layout
* [Grid](#grid)
* [Media Object](#media-object)
* [Responsive Utilities](#responsive-utilities)

# Usage and Examples

## Layout

## Grid
	[row]
		[column sm="6"]
			...
		[/column]
		[column sm="6"]
			...
		[/column]
	[/row]

Flexbox columns are supported by using "flex" rather than a column width.

    [row]
			[column xs="flex"]
				...
			[/column]
			[column xs="flex"]
				...
			[/column]
    [/row]

The container component is also supported in case your theme doesn't include a container.

	[container]
		[row]
			[column sm="6"]
				...
			[/column]
			[column sm="6"]
				...
			[/column]
		[/row]
	[/container]

The container-fluid component is supported as a discrete shortcode.

	[container-fluid]
		[row]
			[column sm="6"]
				...
			[/column]
			[column sm="6"]
				...
			[/column]
		[/row]
	[/container-fluid]

### [container] parameters
Parameter | Description | Required | Values | Default
--- | --- | --- | --- | ---
class | Any extra classes you want to add | optional | any text | none
data | Data attribute and value pairs separated by a comma. Pairs separated by pipe. | optional | any text | none

### [container-fluid] parameters
Parameter | Description | Required | Values | Default
--- | --- | --- | --- | ---
class | Any extra classes you want to add | optional | any text | none
data | Data attribute and value pairs separated by a comma. Pairs separated by pipe. | optional | any text | none

### [row] parameters
Parameter | Description | Required | Values | Default
--- | --- | --- | --- | ---
class | Any extra classes you want to add | optional | any text | none
data | Data attribute and value pairs separated by a comma. Pairs separated by pipe. | optional | any text | none

### [column] parameters
Parameter | Description | Required | Values | Default
--- | --- | --- | --- | ---
xs | Size of column on extra small screens (less than 768px) | optional | 1-12, flex | none
sm | Size of column on small screens (greater than 768px) | optional | 1-12, flex | none
md | Size of column on medium screens (greater than 992px) | optional | 1-12, flex | none
lg | Size of column on large screens (greater than 1200px) | optional | 1-12, flex | none
xl | Size of column on extra large screens (greater than 1200px) | optional | 1-12, flex | none
offset_xs | Offset on extra small screens | optional | 1-12 | none
offset_sm | Offset on small screens | optional | 1-12 | none
offset_md | Offset on column on medium screens | optional | 1-12 | none
offset_lg | Offset on column on large screens | optional | 1-12 | none
offset_xl | Offset on column on extra large screens | optional | 1-12 | none
pull_xs | Pull on extra small screens | optional | 1-12 | none
pull_sm | Pull on small screens | optional | 1-12 | none
pull_md | Pull on column on medium screens | optional | 1-12 | none
pull_lg | Pull on column on large screens | optional | 1-12 | none
pull_xl | Pull on column on extra large screens | optional | 1-12 | none
push_xs | Push on extra small screens | optional | 1-12 | none
push_sm | Push on small screens | optional | 1-12 | none
push_md | Push on column on medium screens | optional | 1-12 | none
push_lg | Push on column on large screens | optional | 1-12 | none
push_xl | Push on column on extra large screens | optional | 1-12 | none
class | Any extra classes you want to add | optional | any text | none
data | Data attribute and value pairs separated by a comma. Pairs separated by pipe. | optional | any text | none

[Bootstrap 4 grid documentation](http://getbootstrap.com/layout/grid/).

* * *

## Media Object
	[media]
		[media-object]
			...
		[/media-object]
		[media-body]
		  [media-heading] ... [/media-heading]
			...
		[/media-body]
	[/media]

## Media List
    [media-list]
		  [media]
			  [media-object]
				  ...
			  [/media-object]
			  [media-body]
			    [media-heading] ... [/media-heading]
				  ...
			  [/media-body]
		  [/media]
			[media]
			  [media-object]
				  ...
			  [/media-object]
			  [media-body]
			    [media-heading] ... [/media-heading]
				  ...
			  [/media-body]
		  [/media]
		[/media-list]

### [media] parameters
Parameter | Description | Required | Values | Default
--- | --- | --- | --- | ---
class | Any extra classes you want to add | optional | any text | none
data | Data attribute and value pairs separated by a comma. Pairs separated by pipe. | optional | any text | none

### [media-object] parameters
Parameter | Description | Required | Values | Default
--- | --- | --- | --- | ---
media | Whether the image pulls to the left or right | optional | left, right | left
alignment | Vertical alignment of the image | optional | top, middle, bottom | top
class | Any extra classes you want to add | optional | any text | none
data | Data attribute and value pairs separated by a comma. Pairs separated by pipe. | optional | any text | none

__NOTE: media-object should contain an image, or linked image, inserted using the WordPress TinyMCE editor__

### [media-body] parameters
Parameter | Description | Required | Values | Default
--- | --- | --- | --- | ---
class | Any extra classes you want to add | optional | any text | none
data | Data attribute and value pairs separated by a comma. Pairs separated by pipe. | optional | any text | none

### [media-heading] parameters
Parameter | Description | Required | Values | Default
--- | --- | --- | --- | ---
class | Any extra classes you want to add | optional | any text | none
data | Data attribute and value pairs separated by a comma. Pairs separated by pipe. | optional | any text | none

__NOTE: media-heading should contain heading tag (h1, h2, h3, h4, h5, or h6), inserted using the WordPress TinyMCE editor. If a header tag is not added h4 will be used__

### [media-list] parameters
Parameter | Description | Required | Values | Default
--- | --- | --- | --- | ---
class | Any extra classes you want to add | optional | any text | none
data | Data attribute and value pairs separated by a comma. Pairs separated by pipe. | optional | any text | none

[Bootstrap media object documentation](http://getbootstrap.com/layout/media-object/)

* * *

## Responsive Utilities
	[hidden down="sm"]
    ...
	[/hidden]g

### [hidden] parameters
Parameter | Description | Required | Values | Default
--- | --- | --- | --- | ---
up | Hide the contents on this screen size and above | optional | xs, sm, md, lg, xl | none
down | Hide the contents on this screen size and below | optional | xs, sm, md, lg, xl | none
class | Any extra classes you want to add | optional | any text | none
data | Data attribute and value pairs separated by a comma. Pairs separated by pipe. | optional | any text | none

[Bootstrap media objects documentation](http://getbootstrap.com/layout/responsive-utilities/)

* * *

### Buttons
Wrap any link in `[button]` to give it button properties and classes.

	[button type="primary"] ... [/button]

Set button sizes with the `size` parameter

    [button type="primary" size="lg"] ... [/button]

Set `block` flag  for block-style buttons

		[button type="primary" block] ... [/button]


#### [button] parameters
Parameter | Description | Required | Values | Default
--- | --- | --- | --- | ---
type | The type of the button | optional | default, primary, success, info, warning, danger, link | default
:triangular_flag_on_post: block | Flag whether the button should be a block-level button | optional | N/A | false
:triangular_flag_on_post: disabled | Flag whether the button be disabled | optional | N/A | false
size | The size of the button | optional | sm, lg | none
class | Any extra classes you want to add | optional | any text | none
data | Data attribute and value pairs separated by a comma. Pairs separated by pipe. | optional | any text | none

[Bootstrap button documentation](http://getbootstrap.com/css/#buttons)

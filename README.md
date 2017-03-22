
# wrapper: Plugin API Docs

<br>

|                      | &nbsp; 
| -------------------- | ---------------------------------------------------------------
| __Type__             | [Library](http://docs.coronalabs.com/api/type/Library.html)
| __Download__         | [wrapper](http://store.coronalabs.com/plugin/wrapper)
| __Sample Code__      | [wrapper sample](https://github.com/sunmils/corona-wrapper-plugin-sample-code)

<br>

## Overview

The plugin allows you to wrap text of a variable length easily to a desired width and height. Varying text will always fit a tutorial window or speech bubble with the best possible font size.

## Features
- Automatic calculated font size
- Custom linebreaks
- "left", "center", "right" and "justify" alignment
- Custom font, font color and line space

View the wrapper.newParagraph() docs and the sample code for detailed instructions.

<br>

## Syntax

	local wrapper = require "plugin.wrapper"


### Functions

##### [wrapper.newParagraph()](newParagraph.md)

<br>

## Project Configuration

### Corona Store Activation

In order to use this plugin, you must activate the plugin at the [Corona Store](http://store.coronalabs.com/plugin/wrapper).


### SDK

When you build using the Corona Simulator, the server automatically takes care of integrating the plugin into your project. 

All you need to do is add an entry into a `plugins` table of your `build.settings`. The following is an example of a minimal `build.settings` file:

``````
settings =
{
	plugins =
	{
		-- key is the name passed to Lua's 'require()'
		["plugin.wrapper"] =
		{
			-- required
			publisherId = "it.eaze",
		},
	},		
}
``````

### Enterprise

If you have activated this plugin, you can download this plugin from the corresponding plugin page in the [Corona Store](http://store.coronalabs.com/plugin/wrapper).

<br>

## Resources

### Sample Code

You can access sample code [here](https://github.com/sunmils/corona-wrapper-plugin-sample-code).

<br>
## Compatibility

Runs on all platforms.

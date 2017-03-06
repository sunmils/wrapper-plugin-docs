
# wrapper: Plugin API Docs

|||
|:--|:--|
| __Type__             | [Library](http://docs.coronalabs.com/api/type/Library.html)
| __Download__         | [wrapper](http://store.coronalabs.com/plugin/wrapper)
| __Sample Code__      | [wrapper sample](https://github.com/sunmils/corona-wrapper-plugin-sample-code)

<br>

## Overview

The wrapper plugin allows you to wrap a text with a variable length into a desired with and height. Different text will always fit a t utorial window or speech bubble, for example.

<br>

## Syntax

	local wrapper = require "plugin.wrapper"


### Functions

##### [wrapper.newParagraph()](newParagraph.markdown)

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

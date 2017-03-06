# wrapper.newParagraph()

|                      | &nbsp; 
| -------------------- | ---------------------------------------------------------------
| __Type__             | [function](http://docs.coronalabs.com/api/type/Function.html)
| __Library__          | [wrapper.*](Readme.markdown)
| __Return value__     | [display object](https://docs.coronalabs.com/api/type/DisplayObject/index.html)



## Overview

What you get with the newParagraph-function is a normal display-group with text objects inside.

Use "\n" within your text to force line breaks.

Study the sample-code and the parameter- and function-List for usage.


## Syntax

	wrapper.newParagraph( parameter )


The `parameter` table contains the following properties:

##### text <small>(required)</small>
_[string](https://docs.coronalabs.com/api/library/string/find.html)._ The text to display.

##### width <small>(optional)</small>
_[number](https://docs.coronalabs.com/api/type/Number.html)._ The desired width of the paragraph. 

##### height <small>(optional)</small>
_[number](https://docs.coronalabs.com/api/type/Number.html)._ The desired height of the paragraph. If a height is set, the fontsize will be ignored and appointed automatically.

##### font <small>(optional)</small>
_[string](https://docs.coronalabs.com/api/library/string/find.html)._ The desired font.




## Examples

``````lua
local myParagraph = Wrapper.newParagraph({

	text = "Wrapper Class Sample-Text\n\nCorona's framework dramatically increase productivity. \n\nTasks like animating objects in OpenGL or creating user-interface widgets take only one line of code, and changes are instantly viewable in the Corona Simulator.",
	width = 400,
	height = 400,                   	-- fontSize will be calculated automatically if set 
	font = native.systemFont, 		-- make sure the used font is installed on your system
	--fontSize = 30,			-- not needed if height is set 	
	lineSpace = 2,
	alignment  = "center",
	
	-- Parameters for speed tweaking, just relevant if height is set
	fontSizeMin = 8,
	fontSizeMax = 30,
	incrementSize = 2
})

--displays the time needed for wrapping
timeText = display.newText(tostring(system.getTimer() - t) .. " ms", 0, display.contentHeight - 22, nil, 20)
timeText.anchorX = 0
timeText.x = 10

myParagraph.anchorChildren = true
myParagraph.anchorX = 0.5
myParagraph.anchorY = 0
myParagraph.x = _W/2
myParagraph.y = 70


myParagraph:setTextColor({0,1,0})


``````

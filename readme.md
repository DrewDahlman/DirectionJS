##DirectionJS
A simple javascript utility for detecting swipe direction and getting feedback of position.

##Use
<pre>
	var _demoElement = new direction(
		'element_id', // Element to watch
		min_movement, // Min Movement to get direction
		dragging_callback, // Dragging Callback
		end_callback // End Callback
	);
</pre>

DirectionJS needs a threshold for movement, this is helpful when you may want to enable snapping of elements back to original position or to their next position based on how much movement has happened.


##Dragging Callback
When a finger begins to swipe on the target element it will return the following data:
<pre>
X: X position of the drag
Y: Y position of the drag
direction: the current drag direction
</pre>

##End Callback
When a finger begins to swipe on the target element it will return the following data:
<pre>
X: X position at end of drag
Y: Y position at end of drag
direction: the drag direction
</pre>
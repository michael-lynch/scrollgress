#Scrollgress

Inspired by [Pitchfork](http://pitchfork.com/features/staff-lists/9466-the-top-200-tracks-of-2010-2014/), Scrollgress is a simple, lightweight jQuery plugin used to display a progress bar at the top of the page that fills up as the user scrolls.

Progress can be measured as the user scrolls the page or an element that has `overflow: scroll | auto` or `overflow-y: scroll | auto`.

<a href="http://michael-lynch.github.io/scrollgress/" target="_blank">See a demo</a>

<a href="http://michael-lynch.github.io/scrollgress/overflow.html" target="_blank">See a demo using an overflow element</a>

##Instructions

Include jQuery and the plugin in the head or footer of your page.

```html
<script src="//ajax.googleapis.com/ajax/libs/jquery/2.1.1/jquery.min.js"></script>

<script src="/js/plugins/scrollgress.js"></script>
```
    
Initialize the plugin targeting the class, ID or element that you want to display the scroll progress of. 

```js
$('body').scrollgress();
```
	
####Options

<ol>

<li>
height: "Npx"
<br />A string that defines the height of the progress bar in pixels (default: '5px').
</li>

<li>color: color
<br />A string that defines the color of the progress bar (default: '#ff0000'). 
</li>

<li>success: function()
<br />A callback function that runs after scrollgress has been initiated (default: function()). 
</li>

</ol>

#####Example:

```js
$(function() {
	
	$('.post').scrollgress({
		height: '10px',
		color: '#990000',
		success: function() {
			console.log('Scrollgress has been initiated.');
		}
	});
		
});
```		
MavSelectBox
============

MavSelectBox is a simple-to-use form select replacement that allows for better customization. I had the need for this myself and all though there are a few out there that do a damn good job, none were exactly what i felt i needed. And as we all know, competition breeds innovation, right?

MavSelectBox mimics the GUI interactions of a normal select element as much as possible (the non-annoying anyway). This is done so as not to break with user expectations. Up and down arrows move the selection, tabbing to it and hitting alt+down shows the menu, tabbing to it and simply hitting up or down selects the next available option in that direction, focusing then start typing and the option that matches what you are typing is selected, enter selects, esc closes, and so on. 


How to use
----------

*HTML*
	#HTML
	<select id="select_field" class="some_class" style="width:200px">
		<option value="first" class="bland">First option</option>
	
		<option value="second" style="color:red">Second-best option</option>
		<optgroup label="Optgroups are hip">
			<option value="opty" class="optful">First optgroup option</option>
	
			<option value="" disabled="disabled">I be disabled option!</option>
	
		</optgroup>
		<option value="thirdee" selected="selected">Selected third!</option>
	
		<option value="lastestes" class="bright sweet" >lastest and Bestest</option>
	</select>

*JS*
	#JS
	var your_select = new MavSelectBox({
		elem: $('another_id'),
		alternate: true,
		onSelect: function(_elem) {
			// Do somethin' funky!
	
		}
	});



Screenshots
-----------

![Screenshot1](http://github.com/dcdustin/MavSelectBox/raw/master/mavselectbox.jpg)

<h1>jQuery</h1>
jQuery: most popular JavaScript tool
* <code>script</code> element:browser will run any JavaScript inside a
script element, including jQuery.
```
<script>
  $(document).ready(function(){
    //here will run as soon as your browser has loaded your page.
    });
</script>
```
**All jQuery functions start with a ```$```, usually referred to
as a ```dollar sign operator``` or ```bling```**

<b>Example</b>)<br>
<code>$("button").addClass("animated bounce")</code> : make all of button elements bounce.<br>
-> You are using jQuery to apply the Animate.css <code>bounce</code> class to your ```button``` element

* ```addClass()``` function:<br>
Allows you to add classes to elements.

* ```removeClass()``` function:<br>
Remove classes to element.

* ```.css()``` function:<br>
Allow you to change the CSS of an element
<b>Example</b>)Change color to blue<br>
```
$("#target1").css("color", "blue");
```

* ```.prop()``` function:<br>
Allow you to adjust the properties of elements(non-CSS properties).<br>
<b>Example</b>)Disable all buttons<br>
```
$("button").prop("disabled", true);
```

* ```.html()``` function:<br>
Let you add HTML tags and text within an element.<br>
<b>Example</b>)Rewrite and italicize the text of heading<br>
```
$("h3").html("<i>jQuery Playgound</i>");
```

* ```.text()``` function:<br>
Alter text without adding tags.<br>

* ```.remove()``` function:<br>
Remove an HTML element entirely.<br>

* ```appendTo()``` function:<br>
Allow you to select HTML elements and append them to another element.<br>
<b>Example</b>)Move ```target4``` from our right well to our left well<br>
```
$("#target4").appendTo("#left-well");
```

* ```clone()``` function:<br>
Make a copy of an element<br>
<b>Example</b>)Copy ```target2``` from ```left-well``` to ```right-well```<br>
**Example**)<br>
<code>
$("#target2").clone().appendTo("#right-well")
</code><br><br>

* ```parent()``` function:<br>
Allow to access the parent of whichever element your've selected.<br>
**Example**)Give the parent element of the ```left-well``` element a background color of blue<br>
```
$("#left-well").parent().css("background-color", "blue");
```

* ```children()``` function:<br>
Allow you to access the children of whichever element you've selected.<br>
**Example**)<br>
```
$("#left-well").children().css("color", "blue");
```

* ```target:nth-child(n)``` css selector:<br>
Allow you to select all the nth element with the target class or element type<br>
**Example**)<br>
```
$(".target:nth-child(3)").addClass("animated bounce")
```

* Target all the even-numbered elements<br>
```
$(".target:odd").addClass("animated shake");
```

* Target the ```body``` element<br>
```
$("body").addClass("animated fadeOut");
```

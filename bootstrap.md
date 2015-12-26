<h1>Boostrap</h1>
* Figure out how wide your screen is and respond by resizing your HTML elements.
* It will look good on devices with screens of any width.
* You can add Bootstrap to any app just by including it by adding the following code to the top of your HTML:
```
<link rel="stylesheet" href="//maxcdn.bootstrapcdn.com/bootstrap/3.3.1/css/bootstrap.min.css"/>
```

<b>nest all of our HTML in a <code>div</code> element with the class <code>container-fluid</code></b>

### Make Images Mobile Responsive
Add the <code>img-responsive</code> class to your Images<br>
-> perfectly fit the width of your page.

### Center Text with Bootstrap
Add class <code>text-center</code> to our <code>h2</code> element</br>

### Create a Bootstrap Button
<b>Bootstrap has its own styles for <code>button</code> element which look much better than the plain HTML ones.</b><br><br>
<b>Add <code>btn</code> class to your button.</b>

* <code>btn-block</code> class:<br>
Button will stretch to fill your page's entire horizontal space and any elements following it will flow onto a new line below the block.
<br>

* <code>btn-primary</code> class:<br>
Use main color you'll use in your app.

* <code>btn-info</code> class:<br>
Call attention to optional actions that the user can take.

* <code>btn-danger</code> class:<br>
Notify users that the button performs a destructive action, such as deleting.

### Use the Bootstrap Grid to Put Elements Side By Side
<b>Bootstrap uses a responsive grid system, which makes it easy to put elements into rows and specify each element's relative width.
* <code>col-md-\*</code> class:<br>
The column width of an element on a medium-sized screen is being specified.

* <code>col-xs-\*</code> class:<br>
The column width of an element on a extra small sized.<br>
<b>Example</b>)
```
<div class="row">
  <div class="col-xs-4"><button class="btn btn-block btn-primary">Like</button></div>
  <div class="col-xs-4"><button class="btn btn-block btn-info">Info</button></div>
  <div class="col-xs-4"><button class="btn btn-block btn-danger">Delete</button></div>
</div>
```

### Add Font Awesome Icons to our buttons
<b>Font Awesome is a convenient library of icons. These icons are vector graphics, stored in the <code>.svg</code> file format. You can specify their size using pixels, and they will assume the font size of their parent HTML elements.<br><br>

The <code>i</code> element turn into an icon.<br>
Example)<br>
<code><i class="fa fa-into-circle"></i>

### Create Bootstrap Wells
* <code>well</code> class:<br>
create a visual sense of depth for your columns.
Example)<br>
```
<div class="well" id="left-well">
```

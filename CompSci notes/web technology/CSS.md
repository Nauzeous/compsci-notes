CSS stands for ==Cascading Style Sheets== and describes how HTML elements are displayed on screens

CSS allows developers to control the layout of **multiple web pages at once**

CSS code can be embedded directly in a HTML file in a \<style> tag, but it will only affect the style of that page

by using separate, external sheets, you can change the look of an entire site by changing one file

external CSS files are linked to an HTML file using the \<link> tag

The exam spec involves the following CSS properties:
- background-color
- border-color
- border-style
- border-width
- color
- font-family
- font-size
- height
- width

CSS inside elements looks like
\<h1 style = "color:red;">
or 
\<h2 style = "border-style:dotted;border-color:blue;">
or
\<h3 style = "font-family:Arial,Helvetica,sans-serif;">

in a separate CSS file it would look more like
h1{
	color:red;
	background-color:yellow;
}
h2 {
	border-style:dotted;
	border-color:blue;
	border-width:thick
}
h3 {
	font-family:Arial,Helvetica,sans-serif;
	color: #00ff00
}

CSS also contains [[OOP|classes]] 
.intro {
	color:red;
	font-size:25px;
}
.main {
	color:green
	font-size:15px
}

classes can be referenced using the \<div class = "classname"> tag in html, so you can reuse the same style several times just by referencing the class

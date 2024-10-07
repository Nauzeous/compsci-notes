HTML stands for ==Hyper Text Markup Language==, the standard markup language for web pages

HTML elements are the building blocks of html and are shown by <>

HTML elements can have attributes that provide additional information about the element

attributes come in name value pairs like ==width = 400==

web browsers interpret the tags to visually render the page

18 different tags in the exam spec:
\<html>
\<link>
\<head>
\<title>
\<body>
\<h1>
\<h2>
\<h3>
\<img>
\<div>
\<a>
\<form>
\<input>
\<p>
\<li>
\<ol>
\<ul>
\<script>

html elements usually have ==start and end tags== with content in between

the end tag is represented with a forward slash before the tag

like \<h1> this is a heading \</h1>

The whole document begins with \<html> and ends with \</html>
Then a \<head> tag  contains metadata, such as the title of the html document when displayed by the web browser
The content displayed by the webpage is held within the \<body>

the  \<p> tag is used to represent a new paragraph, creating a separation between text

the \<img> tag is used to embed an image in the HTML document
images are not inserted into a web page but instead link to another page

by using the tag a space is created for an **image reference**
the tag requires two attributes:
1. src - specify the file path of the image
2. alt - specify alternate text for the image if it cannot be displayed
To control the size of the image specify width and height, otherwise the image will load in it's native resolution

The \<a> tag defines a hyperlink, used to link one page to another using ==href==, short for **hyperlink reference**
ie. \<a href = "https://image.co.uk">
hyperlinks will always be underlined and will be blue when unvisited, purple when visited, and red when active

\<ul> and \<ol> both signify a list, for an unordered list and an ordered list respectively
for a new list item the tag \<li> is used,  short for **list item**
ordered lists are displayed with numbers
1. item 1
2. item 2
3. item 3
whereas unordered lists have bullet points
- item 1
- item 2
- item 3

\<link>, \<div>, \<form>, \<input> and \<script> are linked to CSS and JavaScript


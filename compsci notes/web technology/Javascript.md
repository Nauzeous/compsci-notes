Javascript is the main programming language for the web and is used to modify HTML and CSS

Javascript lets you ==calculate, manipulate and validate data==, controlling the behaviour of the web page

Javascript is implemented by using <\script> and <\form> 

<\form> is used alongside Javascript to process input

a form tag would be implemented like

	 <form id = "form1" action = "/action_page.php">
	 ~Javascript here~
	 </form>


the **action** tells the browser to send submitted form data to a page called action_page.php
the .php file handles server processing of form data

input can be taken using text boxes and buttons by using <\input>

	 <input type = "text" id = "forename" name = "forename">

for a button it would look like

	 <input type="submit" id="Submit" name="Submit" value="Submit">

for data outside a form a <\button> can be used

	 <button onclick = "function()"><\button>

this lets you reference a defined function in Javascript, that must be written somewhere else, inside a set of <\script> tags 

Javascript syntax notes:
- lines end with a **semi colon**
- indentation is marked by braces "{ }"
- types are declared, ie.
> function MyFunction() {}
> 	var x = 12;
> 	var i;
> 	for (i = 0; i != 12; i++) {
> 		x = x + i;
> 	}
> }

- you can write directly do the document using document.write("text") or alert("text")


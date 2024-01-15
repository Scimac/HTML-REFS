### HTML Form
- An **HTML form** is _a section of a document_ which contains controls such as text fields, password fields, checkboxes, radio buttons, submit button, menus etc.

```
<form action="server url" method="get|post" autocomplete="on|off">  
  //input controls e.g. textfield, textarea, radiobutton, button  
</form>  
```

#### Elements under `<form>` tag - 
- The HTML `<input>` element is the most used form element. 

	An `<input>` element can be displayed in many ways, depending on the type attribute, viz. text, password, date, checkbox, submit (shows a button for form submission).
	
	if we are using the action attribute of `<form>` tag, each input field must have a `name` attribute to be submitted. If the `name` attribute is omitted, the value of the input field will not be sent at all in the service as payload.

	Some important attributes of input element - 
		- `readonly`
		- `disabled`
		- `size="50"` -- default size is 20.
		- `maxlength="4"` -- specifies maximum letters allowed to input
		- `min` and `max` attributes specify the minimum and maximum values for an input field.
		- `multiple`
		- `pattern="[A-Za-z]{3}"` attribute specifies a regular expression that the input field's value is checked against
		- `placeholder="123-45-678"`
		- `required`
		- `autofocus`
		- 

- The `<label>` tag defines a label for many form elements. 

	**Majorly helpful for screen-reader users, because the screen-reader will read out loud the label when the user focus on the input element.**
	
	The `for` attribute of the `<label>` tag **should be same as** the `id` attribute of the `<input>` element to bind them together. 
		
		E.g When the user clicks the text within the `<label>` element, it toggles the radio button/checkbox.

- The `<select>` element defines a drop-down list. `selected` attribute will preselect that option. `size` specifies the dropdown size. `multiple` allows the user to select multiple values 

	```
	<select id="cars" name="cars" size="3" multiple>  
	  <option value="volvo" selected >Volvo</option>  
	  <option value="saab">Saab</option>  
	  <option value="fiat">Fiat</option>  
	  <option value="audi">Audi</option>  
	</select>
	```

- The `<textarea>` element defines a multi-line input field (a text area). The `rows` attribute specifies the visible number of lines in a text area. The `cols` attribute specifies the visible width of a text area.

- The `<button>` element defines a clickable button. **Always specify the `type` attribute for the button element. Different browsers may use different default types for the button element.**

- The `<fieldset>` element is used to group related data in a form. The `<legend>` element defines a caption for the `<fieldset>` element.

- The `<datalist>` element specifies a list of pre-defined options for an `<input>` element. Users will see a drop-down list of the pre-defined options as they input data. The `list` attribute of the `<input>` element, must refer to the `id` attribute of the `<datalist>` element.

	```
	<form action="/action_page.php">  
	  <input list="browsers">  
	  <datalist id="browsers">  
	    <option value="Internet Explorer">  
	    <option value="Firefox">  
	    <option value="Chrome">  
	    <option value="Opera">  
	    <option value="Safari">  
	  </datalist>  
	</form>
	```


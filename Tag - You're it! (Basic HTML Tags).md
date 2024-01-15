### Let's visit some important tags

#### Head tag
- The HTML `<head>` element is used as a container for metadata (data about data). 
- Metadata defines the document title, character set, styles, links, scripts, and other meta information.

- Following is a list of tags used in metadata:
	-   `<title>` : It is used in all HTML/XHTML documents. It defines a title in the browser tab, a title for the page when it is added to favorites, a title for the page in search engine results.
	
	-   `<style>` : This tag holds the CSS for the HTML page.
		```
			<style>  
				body {background-color: pink;}  
				h1 {color: red;}      
				p {color: blue;}  
			</style>
		```

	-   `<meta>` : The `<meta>` element is typically used to specify the character set, page description, keywords, author of the document, and viewport settings.
		
		**Define the character set used:**
		`<meta charset="UTF-8">`

		**Define keywords for search engines:**
		`<meta name="keywords" content="HTML, CSS, JavaScript">`
		
		**Define a description of your web page:**
		`<meta name="description" content="Free Web tutorials">`
		
		**Define the author of a page:**
		`<meta name="author" content="John Doe">`
		
		**Refresh document every 30 seconds:**
		`<meta http-equiv="refresh" content="30">`
		
		**Setting the viewport to make your website look good on all devices:**
		`<meta name="viewport" content="width=device-width, initial-scale=1.0">`
		- ##### Importance of the ViewPort:
			* The viewport is the user's visible area of a web page. It varies with the device - it will be smaller on a mobile phone than on a computer screen.
			* The `width=device-width` part sets the width of the page to follow the screen-width of the device (which will vary depending on the device).
			* The `initial-scale=1.0` part sets the initial zoom level when the page is first loaded by the browser.
	
	-   `<link>` : The HTML `<link>` element is used to link an external style sheet to your webpage. The `<link>` element contains main two attributes which are `rel` and `href`. 
		The `rel` attribute indicates that it is a stylesheet, & `href` gives the path to that external file.
		
		`<link rel="stylesheet" href="style.css">  --- self closing, no need for closing tag`
		
	-   `<script>` : [[HTML with JS | The HTML <script> tag is used to define a client-side script (JavaScript). It can be used in <head> as well as <body> tag.]]

	-   `<base>` : The `<base>` element specifies the base URL and/or target for all relative URLs in a page and must have either an `href` or a `target` attribute present, or both.
		
		There can only be one single `<base>` element in a document!


#### Anchor tag
- `<a href = "..........." target="_blank"> Link Text </a>`
	- `href` - specifies the location to redirect the page to
	- `target` - specifies where the page will open

#### Image tag
- `<img src="file path/hyperlink" height="180" width="300" alt="Alternate text">`
	- Always try to insert the image with height and width, else it may flicker while displaying on webpage.

#### Table Tag
```
	<table>  
		<tr>  
			<th>1 header</th>  
			<th>1 header</th>  
			<th>1 header</th>  
		</tr>  
		<tr>  
			<td>1data</td>  
			<td>1data</td>  
			<td>1data</td>  
		</tr>  
		<tr>  
			<td>2 data</td>  
			<td>2 data</td>  
			<td>2 data</td>  
		</tr>  
		<tr>  
			<td>3 data</td>  
			<td>3 data</td>  
			<td>3 data</td>  
		</tr>  
	</table>
```

- A table to display data in tabular form, using `<table>` element, with the help of `<tr>` , `<td>`, and `<th>` elements.
-  `rowspan` and `colspan` attributes of the `<td>` tag are used to 'merged' the cells containing that data. 
- `rowspan` specifies how many rows a cell block with specified rowspan will cover and `colspan` specifies how many column will the cell block cover.

- The following image shows the effect of the `rowspan` and `colspan` -
```
	<td rowspan="3">
	</td><th colspan="2"></th>
```

![[Pasted image 20221005175939.png | 100]]

#### Lists Tags
- There are three different types of HTML lists:
	1. ** Ordered List or Numbered List (ol)**
		```
		<ol>  
			 <li>Aries</li>  
			 <li>Bingo</li>  
			 <li>Leo</li>  
			 <li>Oracle</li>  
		</ol>  
		```
		- All the list items are marked with numbers by default., Hence, also called numbered list.
	2. **Unordered List or Bulleted List (ul)**
		```
		<ul>  
			 <li>Aries</li>  
			 <li>Bingo</li>  
			 <li>Leo</li>  
			 <li>Oracle</li>  
		</ul>
		```
		- All the list items are marked with bullets by default, Hence, also called bulletted list.
		- `<ol type="1" start="5" reversed >` 
			- type - defines the bullets that will be rendered in the list
			- start - defines from where the bullets start
			- reversed - renders bullets/numbers in reverse orders
	1.  **Description List or Definition List (dl)**
		```
		<dl>  
		  <dt>Aries</dt>  
			  <dd>-One of the 12 horoscope sign.</dd>  
		  <dt>Bingo</dt>  
			  <dd>-One of my evening snacks</dd>  
		  <dt>Leo</dt>  
			  <dd>-It is also an one of the 12 horoscope sign.</dd>  
		  <dt>Oracle</dt>  
			  <dd>-It is a multinational technology corporation.</dd>   
		</dl>  
		```

#### Images
- `<img src="/images/picture.jpg" alt="Mountain">`


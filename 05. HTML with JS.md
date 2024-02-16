### HTML with JS

- The HTML `<script>` tag is used to define a client-side script (JavaScript). It can be used in `<head>` as well as `<body>` tag.

- **Position is vital as the scripts called in  `<head>` are loaded before rendering of elements and the one in `<body>` are executed after rendering all the elements.** 

	This is important as if the JS functions include reference to DOM elements, it might throw error.

- The `<script>` element either contains script statements, or it points to an external script file through the `src` attribute.

```
<script>  
	document.getElementById("demo").innerHTML = "Hello JavaScript!";  
</script>

<script type="text/javascript" src="URL "></script>
```

- One HTML can have multiple script tags. 
- The HTML `<noscript>` tag defines an alternate content to be displayed to users that have disabled scripts in their browser or have a browser that doesn't support scripts.

```
<script>  
document.getElementById("demo").innerHTML = "Hello JavaScript!";  
</script>  
<noscript>Sorry, your browser does not support JavaScript!</noscript>
```

### HTML - Hypertext MarkUp language

- **HyperText** simply means "Text within Text." And, a **Markup Language** is a computer language that is used to apply layout and formatting conventions to a text document.
- **Tim Berners-Lee** is known as the father of HTML. In the late 1980's , a physicist, Tim Berners-Lee who was a contractor at CERN, proposed a system for CERN researchers.
-  HTML is a case-insensitive language, which means we can use tags either in lower-case or upper-case.

### Description of HTML Example

`<!DOCTYPE>` : It defines the document type or it instruct the browser about the version of HTML.

`<html >`  : This tag informs the browser that it is an HTML document. Text between html tag describes the web document. It is a container for all other elements of HTML except `<!DOCTYPE>`

`<head>` : It should be the first element inside the `<html>` element, which contains the **metadata(information about the document)**. It must be closed before the body tag opens.

`<title>` : As its name suggested, it is used to add title of that HTML page which appears at the top of the browser window.

`<body>` : Text between body tag describes the body content of the page that is visible to the end user. This tag contains the main content of the HTML document.

`<h1>` : Text between `<h1>` tag describes the first level heading of the webpage. we have 6 of them based on the intensity. (Necessary, as it defines where the page folds in editors)

**Headings in HTML helps the search engine to understand and index the structure of web page.** Helps a lot in [[SEO]] and page ranking.

`<p>` : Text between `<p>` tag describes the paragraph of the webpage.

### Building blocks of HTML

![[Pasted image 20221005151923.png | 300]]

`<tag name  attribute_name= "attr_value"> content </ tag name>`

- **Void element** : All the elements in HTML do not require to have start tag and end tag, some elements does not have content and end tag such elements are known as **Void elements or empty elements, unpaired tag**.

Some Void elements are `<br>` (represents a line break) ,` <hr>`(represents a horizontal line), etc.

- For the default display and styling purpose in HTML, all the elements are divided into two categories:
<ol>
	<li>Block Elements</li>
	<li> Inline Elements</li>
</ol>
### Block-level element:
-   These are the elements, which structure main part of web page, by dividing a page into coherent blocks.
-   A block-level element always start with new line and takes the full width of web page, from left to right.

### Inline elements:
-   Inline elements are those elements, which differentiate the part of a given text and provide it a particular function.
-   These elements does not start with new line and take width as per requirement.
-   The Inline elements are mostly used with other elements.

#### Defining the layout of the page
HTML layouts create an individual space for every part of the web page. So that every element can arrange in a significant order.

![[Pasted image 20221011001221.png]]

-   `<header>` - Defines a header for a document or a section
```
<header>  
  <h1 > Page Header Demo </h1>  
</header> 
```

-   `<nav>` - Defines a set of navigation links for the same page or for other pages.
```
<nav >  
	<h1 >Navgation Links</h1>  
	<ul>  
		<li><a href="#">link1</a></li>  
		<li><a href="#">link2</a></li>  
		<li><a href="#">link3</a></li>  
		<li><a href="#">link4</a></li>  
	</ul>  
</nav>
```

-   `<section>` - Defines a separate section of a web page which contains related element grouped together.
```
<section style="background-color:#ff7f50; width: 100%; border: 1px solid black;">  
    <h2>Introduction to HTML</h2>  
    <p>
	    HTML is a markup language which is used for creating attractive web pages
	    with the help of styling
    </p>  
  </section>  
```

-   `<article>` - Defines an independent, self-contained article such as big story, huge article, etc.
```
<article style="width: 100%; border:2px solid black; background-color: #fff0f5;">  
    <h2>History of Computer</h2>  
    <p>Write your content here for the history of computer</p>  
</article>  
```

-   `<aside>` - Defines content aside from the content (like a sidebar)

-   `<footer>` - Defines a footer for a document or a section, mostly contains information about author, copyright, other links, etc.

-   `<details>` - Defines additional details that the user can open and close on demand

-   `<summary>` - Defines a heading for the `<details>` element
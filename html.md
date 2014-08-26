* Tabs for indentation
* Use `-` for word separator for classes, ids (no camel case)
* Lower case tag names and attributes
* Lower camel case for file names
* No space after last attribute
* Absolutely no `javascript` or inline styles
* Line breaks between nested sibling elements
* Omit trailing slash in self-closing elements, e.g. ```<br>``` not ```<br/>```
* Optional closing tags are required, e.g. ```</li>``` or ```</body>```


## CSS and JavaScript includes
Per the HTML5 spec, typically there is no need to specify a type when including CSS and JavaScript files because ```text/css``` and ```text/javascript``` are their respective defaults.

```html
<!-- CSS -->
<link rel="stylesheet" href="main.min.css">

<!-- LESS -->
<link rel="stylesheet/less" href="main.less">

<!-- JavaScript -->
<script src="main.min.js"></script>
```

## Attribute order
HTML attributes should come in this particular order for easier reading of code.
* ```class```
* ```id```, ```name```
* ```data-*```
* ```src```, ```for```, ```type```, ```rel```, ```href```
* ```title```, ```alt```
* ```aria-*```, ```role```


## JavaScript class selectors
When using classes for JavaScript selectors prefix with ```js-```

```html
<!-- Example -->
<span class='js-selector-class class-for-styling'></span>
```

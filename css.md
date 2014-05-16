* Use tabs for indentation
* Put spaces before and after `:`
* Align consecutive `:`
* Put spaces before `{`
* Use only variables for colors
* Lowercase hex color codes `#0f0f0f`
* Use `//` for comments
* Use `-` for word separator for classes, ids
* Lower camel case for file names
* Semi-colon at each line ending
* Use mixins for CSS3 and browser vendor style properties
* Break out .less files by component

Example:
```
@grey : #CCC;
@base : 10px;

.user-details, .group-details {
	padding    : 0;
	list-style : none;
	margin     : ( @base / 2 ) 0 @base 0;
	color      : @grey;

	li {
		margin : @base 0;
	}
}
```

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

## Mixins
Use mixins where available. Bootstrap comes with many different [vendor](http://getbootstrap.com/css/#less-mixins-vendor) and [ultility](http://getbootstrap.com/css/#less-mixins-utility) mixins pre-configured.

```css
/* Good */
.border-top-radius( 0 );
.box-shadow( inset 0 1px 1px rgba( 0, 0, 0, .075 ) );

/* Bad */
border-top-right-radius : 0;
border-top-left-radius  : 0;

-webkit-box-shadow : inset 0 1px 1px rgba( 0, 0, 0, .075 ) ;
box-shadow         : inset 0 1px 1px rgba( 0, 0, 0, .075 ) ;
```

## JavaScript class selectors
In order to separate the functionality from the aesthetics do not style JavaScript selector classes. This means any class beginning with ```js-``` should not have any styling assigned to it. This makes it easier to refactor either the CSS or the JavaScript without breaking the other.

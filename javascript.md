Install these packages for Sublime Text 3
* https://github.com/SublimeLinter/SublimeLinter3
* https://github.com/mdevils/node-jscs/
* https://github.com/roadhump/SublimeLinter-eslint
* https://github.com/SublimeLinter/SublimeLinter-jshint

* `use strict;`
* Absolutely no `eval()` statements
* Variables must be explicitly declared
* No trailing whitespace
* No `console.log()`
* No commented out code
* Use tabs to indent and spaces to align
* Use single quotes
* Lower camel case all `class` members `var, function`
* Upper camel case all `classes` and `constructors`
* Lower camel case packages
* Descriptive variable names
* Prefix internal/private methods and variables with `_`
* Use sugar syntax for all imports except dependencies loaded on demand, a la [commonjs "sugar" syntax](http://requirejs.org/docs/commonjs.html)

## File Names
* lower-case-hyphenated-folder-names
* Folder names are lower-case dash-separated
* Anything that talks about a path should talk hyphenated
* UpperCamelCase all files that export classes (Models, Collections, Views, Controllers, Applications, Modules)
* Test file name should match the file you are testing with a suffix of `Test`
* Marionette Models, Controllers, Routers, and Collections end with their class types
* Marionette Layouts ends with Layout
* Marionette Composite or Collection Views end with `View`
* Marionette Item Views are the same name as their Composite or Collection View and end with `ItemView`
* Template names are lower camel-case, named after their view
* The type of data ( model or collection ) is singular ( e.g. UserCollection, UserModel )


## Spacing & Alignment
**Spaces between colons**
```javascript
{
	'key1' : 'value',
	'key2' : 'value',
}
```

**Spaces after commas**
```javascript
[ 1, 2, 'three' ]
```

**Spaces after flow control keywords `if, for, while, etc.`**
```javascript
if () {
	// stuff
}
```

**Spaces in bracket accessors**
```javascript
myArray[ 0 ]
myObject[ 'weird-name' ]
```

**Function params user pre and post spaces. Function invocation use post spaces.**
```javascript
function ( a, b, c ) {
	// stuff
}
foo( a, b, c );
```


## Code blocks
**Open curly braces on the same line as the declaration and they end the line their on. Closing curly braces start on their own line. exception: empty object declaration `{}`**
```javascript
if () {
	// stuff
}
```

**No inline code blocks**
```javascript
if ( test === 'foo' ) doStuff();
```

**Nor relying on indentation alone**
```javascript
if ( test === 'foo' )
	doStuff();
```

**After 2 key/value pairs in an object or array (generally), line break all key/value pairs.**
```javascript
{ 'a' : 5 }
[ 1, 2, 'three' ]
```

## Object Keys & Values

**Keys in key/value pairs must be quoted**
```javascript
{
	'key1' : 'value',
	'key2' : 'value',
}
```

**Consecutive values in key/value pairs must be horizontally aligned**
```javascript
var a         = 'foo'
var testError = 'lorem';

var foo = {
	'key'       : 'value',
	'longerKey' : 'value',
	'a'         : 'value'
}
```

**Each var is separately declared & assigned `var; var; var; ...`**
```javascript
var a         = 'foo';
var testError = 'lorem';
```


## Comments
* [Markdown Syntax](http://daringfireball.net/projects/markdown/syntax)
* [Groc](http://nevir.github.io/groc/)
* Per custom function
* Complex logic


## Events
* Event names should fit their purpose, e.g. `pageChange` for changing a page.
* When events are emitted as part of an API for external listeners, the class name should be included, e.g. `SimpleMenu:change`.

# select2-selectionTitleAttribute
Extends Select2 v4 plugin by adding an option to disable the title attribute from the selected elements.


## Description ##
The plugin attaches a `title` attribute to the selected elements by default, and there is no configuration option available to disable this behavior. 

The problem can be reproduced in by placing the mouse over the select box (in single selection mode) or over the selected tags (in multiple selection mode):

[![enter image description here][1]][1]
[![enter image description here][2]][2]

[1]: https://i.stack.imgur.com/DXsJc.jpg
[2]: https://i.stack.imgur.com/fgSCr.jpg


## Setup ##
Include the script after Select2 main javascript file:
```html
<script src="select2.js"></script>
<script src="select2-selectionTitleAttribute.js"></script>
```

## Usage ##
Initialize the select2 plugin with the `selectionTitleAttribute` option set to `false`:

```javascript
$("select").select2({
    // other options 
    selectionTitleAttribute: false
});
```

## Demo ##
Demo available on [JsFiddle](http://jsfiddle.net/hr8bqnpn/). 

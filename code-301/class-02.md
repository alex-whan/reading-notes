# Reading 2: jQuery, Events, and The DOM

## Selected notes from readings in *JavaScript & JQuery* by Jon Duckett

### Chapter 7 - jQuery

**jQuery** is a JavaScript library that allows you to find elements using CSS-style selectors, and then act on them with jQuery methods.

1. Find elements using CSS-style selectors:

  * `$()` is used as shorthand for accessing `jQuery()`
  * Create a jQuery object: `$('li.hot')`
    - Using this CSS-style selector of `.hot` will find all `<li>` elements with a class of `hot`

2. Do something with the elements using jQuery methods:

  * `$('li.hot').addClass('complete');`

  * Use jQuery methods (of the jQuery object) to update elements that object contains
    - Above example uses jQuery method `addClass()` to add the `complete` value to the `class` attribute of the elements on the left 

#### Key Similarities and Differences Between jQuery & DOM:

* **Similarities:**
  - Similar to DOM queries in task, but simpler syntax
  - jQuery objects can be stores in variables (like DOM nodes)
  - jQuery methods/properties can be used to manipulate selected DOM nodes

* **Differences:**
  - jQuery is cross-browser - no need for backup code
  - Selecting elements is simpler/more accurate
  - Event handling simplified (one method that works in all major browsers)
  - Methods affect all selected elements (no loops required)
  - Additional methods provided for popular tasks (like animation)
  - Once something is selected, multiple methods can be applied

#### Reasons for Using jQuery

1. Simpler selectors
2. Common tasks written in less code
3. Cross-browser compatibility

#### jQuery Scripts

* **jQuery Scripts** should ideally be placed before the closing `</body>` tag of your HTML:
  - Script doesn't block other things from downloading
  - DOM has already loaded by the time script executes

#### Getting Element Content

* Use jQuery methods to retrieve and update the content of elements:
  1. `.html()` - only retrieves HTML within the first element in matched set, along with its descendants (text + markup)
  2. `.text()` - only retrieves the *content* a selection (although for every element in selection, along with any descendants)

#### Updating Elements

* Four methods that update contents of **all** elements in a jQuery selection:
  1. `.html()`
  2. `.text()`
  3. `.replaceWith()`
  4. `.remove()`

#### Inserting Elements

* Inserting new elements with jQuery involves two steps:
  1. Create the new elements in a jQuery object
  2. Use a method to insert the content into the page at different locations:
    - `.before()` - before selected elements
    - `.after()` - after selected elements
    - `.prepend()` - inside selected elements, after opening tag
    - `.append()` - inside selected elements, before closing tag

#### Getting and Setting Attribute Values

* You can create attributes, or access/update their contents, using these methods:
  1. `.attr()` - gets or sets a specified attribute and value
  2. `.removeAttr()` - removes a specified attribute and value
  3. `.addClass()` - adds a new value to existing value of class attribute (doesn't overwrite existing values)
  4. `.removeClass()` - removes a value from class attribute (leaves other classes intact)


Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
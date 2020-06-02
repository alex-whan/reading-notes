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

#### Order of Execution and Execution Contexts

Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
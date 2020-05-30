# Reading 4: HTML Links, CSS Layout, JS Functions

## Selected notes from readings in *HTML & CSS* by Jon Duckett

### Chapter 4 - Links

**Links** are created with the `<a>` element

* Attribute: `href = 'URL'`
* Link text is whatever is between the `<a></a>` element tags
* Other link examples:
  - `mailto:user@email.com`: starts user's email program and addresses an email to user@email.com
  - `target`: opens link in a new window
  - `#`: targets a specific place on the same page designated with an `#id`

### Chapter 15 - Layout

#### Key Concepts
* `<div>` elements are often used as containing elements to group together sections of a page, i.e.:
  - Header
  - Main
  - Footer
* Browsers display pages in normal flow unless otherwise specified
* Multiple CSS files can be used in one HTML page
* **Float** property moves content to the left or right of the page, and can be used to create multi-column layouts (although columns must have a specified width and this will pull floated elements out of the normal flow of the page)

#### Blocks
* CSS treats each HTML element as if it is its own "box"
* **Block-level** elements start on new lines
  - Examples: `<h1>, <p>, <ul>, <li>`
* **Inline** elements flow in between surrounding text
  - Examples: `<img>, <b>, <i>`
* Width/height can control how much space each box takes up
* Margins, padding, borders, will help separate individual boxes


## Selected notes from readings in *JavaScript & JQuery* by Jon Duckett

### Chapter 3 - Functions, Methods, and Objects

**Functions**: a series of *statements* grouped together to perform a specific task
* Can be re-used to repeat the same task
* Existing code is wrapped in curly braces `{ }` to make a function

**Statements**: the individual instructions/steps in a function

**Calling a Function**: asking a function to perform its task (must be named in order for it to work)

**Code Block**: One or more statements contained within curly braces (no semicolon after closing brace)

**Parameters**: Pieces of information passed to a function to allow it to achieve a task (like *width* or *height*)

**Return Value**: the response/answer given by a function

### Functions

* Naming a function: Function names can be anything, as long as you use the same names whenever you invoke them (cannot be the same as a variable name)

* Functions will be read by JS but won't actually be run until they are invoked

* **Parameters**: Go in the invocations

* **Arguments**: Happen when you actually *call* a function

### Functions in Code: Layout

Top to Bottom:

* TOP: Global Variables
* MIDDLE: Function Declarations
* BOTTOM: Function Invocations

**Function Invocation**: ```functionName();```


Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
# Reading 3: HTML Lists, CSS Boxes, JS Control Flow

## Selected notes from readings in *HTML & CSS* by Jon Duckett

### Chapter 3 - Lists

There are 3 types of **lists** in HTML:

* **Ordered lists** `<ol>`: each item is numbered
* **Unordered lists** `<ul>`: each item is listed with a bullet point
* **Definition lists** `<dl>`: sets of items along with their definitions

* Ordered and unordered lists use **list items** `<li>` to indicate each item in their list

* Definition lists usually have pairs of **definition terms** `<dt>` and **definitions** `<dd>` elements

* All browsers indent lists by default

* Lists can be nested inside one another

### Chapter 13 - Boxes

* CSS treats each HTML element as if it's its own **box**

* Properties of boxes we can control with CSS:
  - Dimensions
  - Borders
  - Margins
  - Padding
  - Show/hide boxes

* Three main properties to control box appearance:

  - **Border**: Separates the edges of a box from another
  - **Margin**: Gap between the borders of a box and others (i.e., the *outside* of the border)
  - **Padding**: Space between the border of a box and any element contained inside (i.e., the *inside* of the border)

## Selected notes from readings in *JavaScript & JQuery* by Jon Duckett

### Chapter 4 - Decisions & Loops

#### Switch Statements

* **Switch statements** are somewhat like a "multi-level version" of if/else statements - which provide better performance than multiple series of if/else statements running

  - Switch statements begin with a variable called the **switch value**
  - Each case indicates a possible value for that variable - and the code that should run if the variable matches that value

  #### IF/Else Statements VS. Switch Statements

  * If/Else statemenets don't necessarily need the *else* option - they can just be "if" statements
  * With multiple if/else statements in a series, *all* of them will be checked even if a match is found
  * Slower performance

  * Switch Statements can have a **default** option to run if no cases match
  * If a match is found, that code runs, and then a **break** statement stops the rest from running
  * Faster performance

  ### More to follow!
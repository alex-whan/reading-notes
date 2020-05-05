# Reading 7: HTML Tables; JS Constructor Functions

## Selected notes from readings in *HTML & CSS* by Jon Duckett

### Chapter 6 - Tables

* **Tables** represent information in grid format
  - Each block within a table is a table **cell**

* Tables are drawn row by row with `<tr>`

* Cells can span multiple rows or columns with th `rowspan` and `colspan` attributes

* Longer tables should be split into multiple parts (`<thead>`, `<tbody>`, `<tfoot>`)

* Must indicate even empty cells with `<th>` and `<td>` elements to allow for proper rendering of a table

#### Table Structure

* `<table>`: Creates a table
* `<tr>`: Table Row
* `<td>`: Table Data (Cell)
* `<th>`: Table Heading
* For longer tables: `<thead>`, `<tbody>`, `<tfoot>`

#### Table Attributes

* `rowspan`: Indicates how many rows a cell should run across
* `colspan`: Indicates how many columns a cell should run across



## Selected notes from readings in *HTML & CSS* by Jon Duckett

### Chapter 3 - Functions, Methods, and Objects

## Objects

**Objects** are representations or models in programming of "things" in the real world, and each object can have its own *properties*, *events*, and *methods* (which work together to create this model)

* These are examples of **name/value pairs**, which are very common in programming and within the structure of a webpage itself (i.e. - in HTML, attributes are like properties, which can each have different names/values)

**Functions**: a series of *statements* grouped together to perform a specific task
* Can be re-used to repeat the same task
* Existing code is wrapped in curly braces ```{ }``` to make a function

#### Variables and Functions take on new names within an object:
  
* Variables become known as **properties**
  - Tell us about an object
  - Example: a hotel's name, or the number of rooms it has

* Functions become known as **methods**
  - Represent tasks that are associated with the object
  - Example: checking how many rooms are available at a hotel by subtracting number of booked rooms from number of total rooms

Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
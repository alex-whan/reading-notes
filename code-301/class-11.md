# Reading 11: EJS

### EJS

**EJS** = **Embedded JavaScript** Templates

* Templating language/engine that allows you to generate HTML markup with plain JavaScript

* Installation: `npm install -S ejs`

* Use in your code:
  - `app.set("view engine", "ejs");`

* EJS is especially useful when:
  - You have to output HTML with a lot of JavaScript
  - Generating dynamic content
  - Updating a page in real-time/offering real-time updates

### EJS Syntax

* `<% code %>` - content inside these brackets will evaluate/run as code
* `<%= item %>` - content inside these brackets will display what the variable is

* Templates/files in EJS are called **views**

* In code, EJS uses `.render()` instead of `.send()` when returning results
  - Example: `response.render('show.ejs', {searchResults: finalBookArray});` 

Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
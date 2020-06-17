# Reading 12: Components & EJS Partials

### EJS Partials

* **Partials** are particularly useful when you'd like to reuse the same HTML across multiple views
  - Think of **partials like functions**: They make larger websites easier to maintain (only have to change text in one place)
  - Define reusable code in a file, and then just include it wherever it's needed

* Basically, **partials are an easy way to utilize reusable text**

* **Partials** are native to EJS (unlike layouts)
  - Usage examples: Nav bar, footer, reusable piece of static text

  * Syntax for partials: 
        `<%- body %>`
        `<%- include('partials/onepartial') %>`
    - This tells EJS to look in a directory called *"partials"* (in the views folder), and will find a file called *"onepartial"*
  
### Partials Put to Use

Real-life example: You have the same nav bar and footer in both the home and post views of your site:

* Under `views/partials/` directory, create new files `navbar.ejs` & `footer.ejs`
  - These files will contain only the HTML for the nav bar at the top and footer at bottom of both of those pages:

            <!-- views/partials/navbar.ejs -->
    <div class="header clearfix">
        <nav>
            <ul class="nav nav-pills pull-right">
                <li role="presentation"><a href="/">Home</a></li>
            </ul>
            <h3 class="text-muted">Node.js Blog</h3>
        </nav>
    </div>


Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
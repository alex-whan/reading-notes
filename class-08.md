# Reading 8: More CSS Layout

## Selected notes from readings in *HTML & CSS* by Jon Duckett

### Chapter 15 - Layout (part II)

* Normal web pages are typically around 960 pixels wide
  - Designers indicate what the site is about within top 600 pixels - so users don't have to scroll

#### Types of Layouts

**Fixed Width Layouts**: Designs don't change as user increases/decreases screen size or browser window.

* Measurements are generally given in **pixels**

* **Pros:**
  - Pixel values accurately control size and position of elements
  - Site will more or less always look the same
  - Designer has greater control over appearance/layout
  - Lines of text can be controlled length-wise regardless of window size
  - Image sizes will always remain the same relative to page

* **Cons:**
  - May end up with big gaps around page edges
  - If a user has a much higher-resolution screen, the page may render extremely small/unreadable
  - Font size increases by the user may cut off text
  - Best for desktop sites (not mobile)
  - Page may take up a lot of vertical space

**Liquid Layouts**: Designs stretch and contract as the user increases/decreases screen size or browser window

* Measurements are generally given in **percentages** (more reactive)

* **Pros:** 
  - Pages expand to fill full browser window - no spaces around the page
  - Page can contract to fit into small user windows without scrolling
  - More tolerant of larger font sizes set by user (page can expand to accommodate them)

* **Cons:**
  - Harder to predict how the site will look - if you don't control the width of page sections, it can end up looking drastically different than intended
  - Wide user windows may result in very long lines of text (i.e., unwrapped)
  - Narrow user windows may result in very squashed text, with only a few words on each line
  - Fixed width items that are bigger than their containing boxes may overflow text/other elements

  #### Layout Grids

  * Designs often use **grid structure** to help them position items on a page and arrange visual elements

  * **960 pixel grid**: a widely-used grid by web developers that superimposes thick vertical lines over the page
    - Helps create/designate columns for elements
    - Column layouts are very diverse, and you can create a large range of layouts using this grid

#### CSS Frameworks

**CSS Frameworks** provide code for common tasks and allow designers to skip writing CSS code from scratch, including:
  - Creating layout grids
  - Styling forms
  - Creating printer-friendly versions of pages

* **Pros:** 
  - Saves you from repeatedly writing code (D.R.Y.!)
  - Already pre-tested across multiple browser versions (fewer bugs)

* **Cons:**
  - Often not optimized for *semantic HTML* - tags control presentation of page, but aren't decriptive of content
  - Often contain more code than needed for a given page - in order to make them widely applicable (can result in **code bloat**)

* **960.GS CSS Framework**
  - Popular framework - provides templates to help design pages using the common 12-column grid
  - See page 391 of CSS book for example photos

Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
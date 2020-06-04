# Reading 4: Responsive Web Design and Regular Expressions

### CSS Grid

**CSS Grid Layout** is considered the most powerful layout system available in CSS
  - 2-D system that can handle **columns and rows**
  - As opposed to flexbox, which is largely 1-D

* Grid layout basics: Apply CSS rules both to a parent element (**grid container**) and to that element's children (**grid items**)

* Flexbox and Grid work well together when combined

* Grid is specifically designed to solve longtime/common layout problems (and most browsers now natively support it)

#### Getting Started with Grid

* To start, you must define a container element with `display: grid`
  - Set column sizes with `grid-template-columns`
  - Set row sizes with `grid-template-rows`
  - Then place child elements into grid with `grid-column` and `grid-row`

* Source order of grid items doesn't matter (similar to flexbox)
  - CSS can control their order, and rearranging grid items with media queries becomes super simple

#### Important Grid Terminology

* **Grid Container:** The element on which `display: grid` is applied (direct parent of all grid items)

* **Grid Item:** The children (direct descendants) of the grid container

* **Grid Line:** The dividing lines that make up the structure of the grid
  - Can be vertical (column grid lines) or horizontal (row grid lines)

* **Grid Cell:** The space between two adjacent row and two adjacent column grid lines
  - A single unit of the grid

* **Grid Track:** The space between two adjacent grid lines
  - Think of them like the columns/rows of grid

* **Grid Area:** The total space surrounded by *four* grid lines
  - May be composed of any number of cells

#### The Most Powerful Lines in Grid

* **Fluid width columns** can break into more or less columns as space is available - without the use of media queries:

          . grid {
            display: grid;
            grid-template-columns: repeat(auto-full, minmax(200px, 1fr));
            grid-gap: 1rem;
          }


#### Grid Properties

* Different properties for Parent elements (Grid Container) and Children (Grid Items)


### Regular Expressions (Regex)

**Regular Expressions**, known as **Regex** or **Regexp**, are tools used for extracting information from any text
  - Basically: *A sequence of characters the define a search pattern*
  - Search for one or more matches of a specific search pattern (i.e. a specific sequence of characters)

* Uses include:
  - Validation
  - Parsing/replacing strings (think 'find and replace')
  - Passing through translating data to other formats
  - Web scraping

Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
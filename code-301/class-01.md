# Reading 1: SMACSS and Responsive Web Design

### Shay Howe's Intro to RWD (Responsive Web Design)

* Key question: How do you build websites suitable for all users - those who use *mobile* and *desktop* platforms?

* **Responsive Web Design (RWD)** has been the industry response to this question
  - This is the practice of building a website that works on every device and screen size, regardless of overall size
  - Dynamically adjusts to different browser/device viewports, and reorganizes content layout accordingly

#### Flexible Layouts

* **Flexible layouts**: the practice of building a website's layout with a flexible **grid** made up of **relative length units** instead of set lengths
  - Generally set using *percentages* or *em* units

* Proportions of flexible grid layout: `target / context = result`
  - Turn all of the fixed units of length into relative units - so that the elements of the page always scale proportionally

* Example CSS code from reading:

        section,
        aside {
          margin: 1.858736059%; /*  10px ÷ 538px = .018587361 */
        }
        section {
          float: left;
          width: 63.197026%;    /* 340px ÷ 538px = .63197026 */   
        }
        aside {
          float: right;
          width: 29.3680297%;  /* 158px ÷ 538px = .293680297 */
        }

#### Media Queries

* **Media queries** provide the ability to specify different styles for specific browser/device circumstances (i.e., orientation, viewport width, etc)

* Media queries use the `@media` rule in CSS3
  - i.e.: `@media all and (min-width: 800px) and (max-width: 1024px);`

* Each query can include a **media type** followed by one or more expressions
  - Media types include: `all`, `screen`, `print`, `tv`, `braille` (default is `screen`)

* **Logical operators** can be used in media queries, including:

  - `and`: Allows for extra conditions to be added
    * `@media all and (min-width: 800px) and (max-width: 1024px)`

  - `not`: Negates query - specifying any query but the one identified
    * `@media not screen and (color)`

  - `only`: Hides styles from devices/browsers that don't support media queries (pre-HTML5)
    * `@media only screen and (orientation: portrait)`

#### Media Features

* **Media features** identify what attributes or properties will be targeted within a media query expression

* Common media features:
  - `height`, `width`
  - `min-width`, `max-width`, `min-height`, `max-height`
  - `orientation:`, (`orientation: landscape`, `orientation: portrait`)
  - `aspect-ratio`, `device-aspect-ratio`, `min-device-aspect-ratio`
  - `pixel-ratio`, `device-pixel-radio`
  - `resolution`, `min-resolution`
  - `color`, `color-index`, `monochrome`

* Media query/feature demo:
          @media all and (max-width: 420px) {
            section, aside {
              float: none;
              width: auto;
            }
          }

* Many designs use a **mobile first** approach
  - Use styles targeted for smaller viewports as the defaults, and then use media queries to add styles as the viewport grows

#### Viewport

* **Viewport**: a meta-tag that helps a website scale to the size of a device screen

* For best results, use device defaults for the viewport:
  - `device-height`
  - `device-width`

### All About Floats

* **Float**: CSS positioning property that essentially allows for "text wrap" - content flowing around the floated element
  - Remain a part of the flow of the page (unlike absolute positioning)

* Floats can be used for page/web layouts
  - HOWEVER: Generally we use **Flexbox** and **Grid** these days as they are more powerful tools overall

* **Clearing** the float (`clear` property) tells an element to stay below a floated element (like a block) rather than floating up next to it

* Multiple methods for clearing floats:
  - Empty Div Method
  - Overflow Method
  - Easy Clearing Method

### Don't Overthink It Grids

### CSS Floats Explained by Riding an Escalator

### SMACSS Official Documentation
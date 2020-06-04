# Reading 3: Flexbox and Templating

### Templating in JavaScript

* **Templating** is a fast and efficient technique to render client-side view templates with Javascript by using a **JSON data** source
  - Templates are put straight into HTML markup
  - Templating tags will insert variables or run programming logic
  - Template engine replaces variables/instances with actual values when run, and then returns these as an HTML file sent to the client

### Templating with Mustache

**Mustache** is a logic-less template syntax
  - Can be used in HTML, config files, and source code, among others
  - Expands tags in a template using values provided in a hash or object
  - "Logic-less": No if statements, else clauses, or for loops - only tags
  - Tags may be replaced with a value, series of values, or nothing

* Syntax: Two sets of curly braces ``{{}}`` indicate that it is a **placeholder**

* When compiling, Mustache will replace the *placeholder* with the actual value:
  - i.e.: `{{name}}` would become `{{Bob}}` if "Bob was passed in as the actual value


### A Guide to Flexbox

**Flexbox** is a layout/module designed to efficiently lay out, align, and distribute space among items in a container on a page
  - Works even when size of items is unknown or dynamic

* Flexbox's main idea is that it gives containers the ability to change the width/height/order of items within them in order to best fill available space
  - Also helps to accommodate all types of screen/device sizes

* **Flex containers** expand and shrink items to fit available free space and prevent overflow

* Flexbox layout is **direction-agnostic** - making it more flexible and simpler to support complex applications with regards to resizing and changing

* Flexbox layout is ideal for components of an application, as well as small-scale layouts (**Grid** is better for larger layouts)


### Flexbox Properties

* The properties below also have multiple different values that can be assigned to them to change their behavior within Flexbox layout

#### Parent element: Flex container

- `display: flex`
- `flex-direction: row | row-reverse | column | column-reverse`
- `flex-wrap: nowrap | wrap | wrap-reverse`
- `flex-flow`
- `justify-content: flex-start | flex-end | start | end | left | right | center | space-between | space-around | space-evenly`
- `align-items: stretch | flex-start | start | self-start | flex-end | end | self-end | center | baseline`
- `align-content: flex-start | flex-end | center | stretch | space-between | space-around`

#### Child elements: Flex items

- `order`
- `flex-grow`
- `flex-shrink`
- `flex basis`
- `flex`
- `align-self`


Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
# Reading 5: HTML Images, CSS Color & Text

## Selected notes from readings in *HTML & CSS* by Jon Duckett

### Chapter 5 - Images

* **Images** are added with the `<img>` tag in HTML
* **Properties of images:**
  - `src`: tells the browser where to find the file (generally a relative URL to an image on your own site) - must always be specified
  - `alt`: text description of the image in case it cannot be displayed or for screen reading software
  - `title`: provides additional image information - generally displayed by browsers when you hover over an image

  - Images also have `height` and `width` properties

* **Three rules for creating images:**
  1. Save images in the right format
  2. Save images at the right size
  3. Measure images in pixels

* **Types of image files**:
  - `JPEGs` - better for photographs
  - `GIFs` - better for illustrations/logos using flat colors

### Chapter 11 - Color

#### Key Concepts
* **Color** is a critical way of bringing websites to life and attract your target audience
* CSS treats each HTML element as if it is in its own "box"
* These boxes can then be colored and modified accordingly
* Color pickers can help you find a specific color
* Contrast between text/background on a page is key to making content readable to visitors

#### Key Color Properties in CSS

* `color`: text (foreground) color
* `background-color`: background color of an element
* `opacity`
* `rgba`
* `hsl` or `hsla`

#### Specifying Color in CSS

There are three different methods for specifying color in CSS:

1. RGB values: These values specify how much red, blue, and green make up a color. 

Example: rgb(100, 100, 10)

2. Hex codes: These six-digit codes represent the amount of red, green, and blue in a color, preceded by a hash/pound.

Example: #ee3e80

3. Color names: These use the names of 147 different predefined colors recognized by browsers.

Example: DarkCyan, Blue, LightBlue

### Chapter 12 - Text

#### Typefaces

* **Serif:** Fonts with extra details on the ends of the main strokes

* **Sans-Serif:** Fonts that have straight ends on the letters for a cleaner design

* **Monospace:** Every letter is the same width (fixed-width) - like in a code editor

* **Cursive**: Either have joining strokes or handwriting-like characteristics

* **Fantasy**: Generally decorative fonts used for titles - not long bodies of text

#### Properties of Text in CSS

* `font-weight`
* `font-family`
* `font-size`
* `text-transform`
* `text-decoration`
* `text-align`
* `text-indent`
* `text-shadow`
* `vertical-align`
* `line-height`
* `style`
* `stretch`

Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
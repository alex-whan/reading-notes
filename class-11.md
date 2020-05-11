# Reading 11: Assorted Topics

## Selected notes from readings in *HTML & CSS* by Jon Duckett

### Chapter 16 - Images

#### Controlling Sizes of Images in CSS

* `height` and `width` properties can control the size of images in CSS

* Specifying image size can help pages load more smoothly - as browsers can render the rest of a page without waiting for an image to download (will take up a known amount of space)

* Many specific image sizes are used specifically across sites designed with grids:
  - Small portrait: 220 x 360 px
  - Small landscape: 330 x 210 px
  - Feature photo: 620 x 400 px

* Good practice to give images classes based on their size (small, medium, large)

#### Aligning Images Using CSS

* `float` property is often used to align images to the left or right of a page

* `align-left` and `align-right` are classes often given to elements - which are then given margins on the left or right

#### Centering Images Using CSS

* Images are inline elements by default

* Turn images into a `block` level element in order to center it

* Methods for centering a block-level image: 
  - Use `text-align` property on the *containing element*
  - Set `margin` properties of the *image* itself to `auto` (or: `margin: 0 auto;`)

#### Background Images

* **Background images** can be used behind any HTML element (by default, images will repeat to fill whole box)

* Important properties:
  - `background-image`
  - `background-repeat`
  - `background-attachment`
  - `repeat-x`
  - `repeat-y`
  - `no-repeat`
  - `fixed`
  - `scroll`
  - `background-position: center top` OR `50% 50%` - can be used to specify where in the window the image should be placed if not repeating

* **Sprite:** A sprite is when a single image is used for several different parts of an interface (can help web page load faster)

### Chapter 19 - Practical Information

#### Search-Engine Optimization (SEO)

* **SEO** ultimately helps visitors find your site via search engines
  - Helps your site appear near the top of search engine results when people look for related topics
  - Essentially, figuring out which search terms people are likely to use to find your site

* **Keywords** will be a big part of this - search engines rely on them heavily for determining relevance
  - Keywords in **links** are especially useful - search engines consider keywords inside <a> tags to be more relevant

#### Analyzing Your Visitors

* **Google Analytics** is a free service that helps you track/visualize how visitors are using your website

* Uses a tracking code embedded in your website (just before the closing `</head>` tag) to provide this data

* Key Info Tracked by Google Analytics (Many more examples in addition to the below):
  - **Visits**: Number of times people have com to your site
  - **Unique Visits**: Total number of different people visiting site over a specific period
  - **Page Views**: Total number of pages all visitors have viewed on your site
  - **Pages Per Visit**: Average number of pages each visitor has looked at
  - **Average Time on Site**: Average time spent on site per visit
  - **Pages**: Which pages visitors are looking at the most and spending the most time on
  - **Landing Pages**: Pages that people arrive on when first visiting (may not always be arriving via homepage)
  - **Top Exit Pages**: Which pages visitors most commonly leave from
  - **Referrers**: Shows sites that have linked to you and the number of visitors coming via those sites
  - **Direct**: Pages users arrived on if they did not come via another site's link
  - **Search Terms**: Shows terms users entered into a search engine to find your site

* Other features:
  - **Date Selector**: Can time-box data to show trends during a specific period
  - **Export**: Export statistics for other applications (like Excel)

  #### Domain Names & Hosting

  * You'll need a **domain name** and **web hosting** in order to put your site on the internet

  * **Domain Name**: Your web address to which the domain is registered (i.e., bbc.co.uk, google.com, etc.)

  * **Web Hosting**: Your website needs to be uploaded to a **web server** in order to be seen by others


Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
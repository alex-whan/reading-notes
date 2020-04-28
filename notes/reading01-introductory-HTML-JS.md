# Reading 1: Introductory HTML & JavaScript

## Selected notes from readings in *HTML & CSS* by Jon Duckett

### Chapter 1 - Structure

#### Key Concepts of Website Structure
* HTML pages are ultimately text documents displaying content
* HTML documents use **tags** to give certain content special meaning/importance
* Tags: special characters written in angled brackets (nearly always in pairs)
* These specially-designated combinations of tagged text/characters are known as **elements**

### Chapter 8 - Extra Markup

#### Key Extra Markup Cheatsheet
* Comments in HTML: ```<!-- -->```
Comments are very important for leaving notes in code that will not show up in the browser, making it much easier to understand your thinking when revising older code or when someone else is reading your code.
* Doctypes: Tells the browser which version of HTML is being used
* ID attribute: Uniquely identifies that element from all others on the page - though no two elements on the same page can have the same unique ID value
* Class attribute: Identifies several different special elements within a document
* Inline, block, and inline-block elements: Organizes content into different spacing/layout on page

### Chapter 17 - HTML 5 Layout

#### Key Features of HTML 5
* New elements that allow for clearer and more effective division of a page
* Element names are more intuitive and self-explanatory
* More specific and specialized layout elements to help demonstrate and describe a page's structure
* These elements also make it easier for accessibility software to discern the most important information on a page

#### Elements of HTML 5
* Headers: ```<header>```
* Footers: ```<footer>```
* Navigation: ```<nav>```
* Articles: ```<article>```
* Asides: ```<aside>```
* Sections: ```<section>```
* Heading Groups: ```<h1> <h2> <h3>```
* Figures & Captions: ```<figure> <figcaption>```
* Divs: ```<div>```

### Chapter 18 - Process and Design

#### Key Website Design Considerations
* Target audience - who is the website *for*?
* What are the requirements and needs of the target audience?
* How do I present the required information/content in an accessible and appealing format?
* What information will the audience need? How often will they need it?
* Do they need generic information, or do they have specific goals?

#### Planning a Website
* Site Map: a diagram/tree of pages to be used on the site and how they will be grouped
* Wire frame: a basic overview/layout of the most critical information that needs to go on each page - helping to visualize needed space


## Selected notes from readings in *JavaScript & JQuery* by Jon Duckett

### Chapter 1/C - How Do I Write a Script for a Web Page?

#### Key Concepts of JavaScript
* JavaScript is the "behavioral layer" of a web page and adds interactivity to the HTML/CSS layers
* JavaScript can be embedded in HTML, but best-practice is to keep JS in a separate file(s) as part of the **separation of concerns**
* JavaScript is written in plain text - no special tools or software are needed to write it
* JavaScript scripts do not change the HTML source code when run

*Content Layer (HTML) --> Presentation Layer (CSS) --> Behavior Layer (JavaScript)*

### Objects & Methods

```document.write('Good Afternoon!');```

This is an example of **calling a method**, which uses the structure seen above of **object.method(parameters)**.

# Programming with JavaScript

## Foundational pieces of JavaScript for Code 201:
* Functions
* Loops
* Arrays
* Conditionals

Computers **only** do what you tell them to do, exactly **how** you tell them to do it, and need **very** specific instructions in order to do so.

## JavaScript Basics

JavaScript makes pages more **interactive**:
* Accesses Content: Selects any element/attribute/text from HTML
* Modify Content: Add elements/attributes/text from HTML
* Program Rules: Specify steps for browser to follow
* React to Events: Specify what script should run when a specific event occurs

Examples of JavaScript in Browsers:
* Slideshows
* Forms
* Reloading/refreshing parts of page
* Filtering data/results

# Objects and Properties

## Objects

**Objects** are representations or models in programming of "things" in the real world, and each object can have its own *properties*, *events*, and *methods* (which work together to create this model)

* These are examples of **name/value pairs**, which are very common in programming and within the structure of a webpage itself (i.e. - in HTML, attributes are like properties, which can each have different names/values)

## Properties

**Properties** are the characteristics of an object

* Each property has its own name and value that give you information about an object's individual **instance**

* In the real world, this could be like make, color, and engine size for a car

* For example: Object Type: `hotel`; Properties: `name`, `rating`, `number of rooms`, `bookings`, `gym (true)`, `pool (false)` 

## Events

**Events** can cause a trigger of certain specific sections of code - and are examples of interactions between users and programming (equivalent to interactions with real-world objects)

* For example: Clicking on a "contact" link on a page might bring up a contact form for a user to fill out

* In the real world, this could apply to car; the brakes slow it down, accelerator speeds it up

* **Scripts** use events to trigger different functionality, and detail events to respond to, as well as which part of the script will run when each event occurs

* For example: Object: `hotel`; Event: `book` - happens when reservation is made; `cancel` - hapens when reservation is cancelled

## Methods

**Methods** represent things people need to do with objects, and can retrieve or update the properties of objects

* Method code can contain lots of instructions to represent one task

* Tell you about onbject using information in properties, *or* changes the value of object's properties

* For example: Object: `hotel`, Method: `makeBooking()` - increases value of the `bookings` property; `cancelBooking()` - decreases value of the `bookings` property

* We don't necessarily need to ask how a method does a task, but rather how to ask questions of it and interpret its answers

## How Does It All Fit Together?

* *Events* can trigger *methods*, which can then retrieve or update the *properties* of an *object*

* For example: Object type: `hotel`
1. Event: `book` - happens when a reservation is made and calls the method `makeBooking()`
2. Method: `makeBooking()` - method increases value of `bookings` property
3. Properties: `bookings` property increases from 21 -> 22

* Web browsers are programs built using objects:
    * `window` object: how the broswer represents each window or tab (`location` property tells us the URL)
    * `document` object: represents the current web page loaded into each window (`title` property tells us what's inside the `<title>` tags, while `lastModified` would tell us when the page was updated
    * For example: 
        * Object type: `window`; properties: `location`
        * Object type: `document`; properties: `URL`, `lastModified`, `title`

## More About the "Document" Object

* The **document** object represents an HTML page - and using this object allows you to access and change what content users see/interact with on it

* A document object has:
    * Properties: i.e., the title of a page
    * Methods: performing document tasks (like getting information from a specific element currently displayed)
    * Events: can respond to events (like a user clicking on an element)

* All major browsers implement the document object in the same way - one of a set of objects that all browsers support

## How a Browser Sees a Webpage

1. Retrieves page as HTML code
2. Creates a model of a page and stores it in its memory
3. Uses a rendering engine to display the page on-screen

**NODE**: Each box below the document object is a node, and *each node is another object*
* i.e.: elements, text within the element, and attribute
* Each element is creates its own node







Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
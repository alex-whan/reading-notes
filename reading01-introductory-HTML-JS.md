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

### Variables

A **variable** is a way for a script to temporarily store data and assign a value that can be recalled at a later time in the same document. Variables are undefined until you assign a value to them.

**Declaring** a variable at the start of a JavaScript document means that a programmer will be able to use the variable later. JavaScript requires variables to be declared before they can be used. This means to essentially give the variable a name.

There are six **rules of naming variables** to keep in mind:

1. Name bust begin with a letter, dollar ($) sign, or underscore (_).
1. Name can contain letters, numbers, dollar signs, or underscores, but NO dashes (-) or periods (.).
1. Cannot use **keywords** or **reserved words** - such as ```var```.
1. Variables are case sensitive.
1. Use a name that describes a variable's data/purpose wherever possible (such as: firstName, lastName, etc).
1. If a variable name is more than one word, capitalize the first letter of each word *after* the first word (such as: firstName, lastName, etc).

### Data Types for Variables

* **Numeric**: Handles numbers only.
* **String**: Letters and other characters (must be within quotation marks - single or double)
* **Boolean**: a simple, binary, TRUE/FALSE value (like an on/off light switch)

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

## Key Concepts

**Scripts**: Scripts are series of instructions for a computer to follow

**Flowcharts**: Sketch out scripts using flowcharts to show paths between each step

**Expressions**: Evaluate/result into a single value
* Expressions that assign a value to a variable
 ```var color = 'beige'```
* Expressions that use two or more variables to return a single value
```var area = 3*2```

**Operators**: Allow expressions to work and programmers to create one value from one or more values
* *Assignment operators* assign value to a variable
``` color = 'beige'```
* *Arithmetic operators* perform basic math
```area = 3*2```
* *String operators* combine two strings
```greeting = 'Hi' + 'Molly';```

**Functions**: a series of *statements* grouped together to perform a specific task
* Can be re-used to repeat the same task
* Existing code is wrapped in curly braces ```{ }``` to make a function

**Statements**: the individual instructions/steps in a function

**Calling a Function**: asking a function to perform its task (must be named in order for it to work)

**Code Block**: One or more statements contained within curly braces (no semicolon after closing brace)

**Parameters**: Pieces of information passed to a function to allow it to achieve a task (like *width* or *height*)

**Return Value**: the response/answer given by a function

### Functions

* Naming a function: Function names can be anything, as long as you use the same names whenever you invoke them (cannot be the same as a variable name)

* Functions will be read by JS but won't actually be run until they are invoked

* **Parameters**: Go in the invocations

* **Arguments**: Happen when you actually *call* a function

### Functions in Code: Layout

Top to Bottom:

* TOP: Global Variables
* MIDDLE: Function Declarations
* BOTTOM: Function Invocations

**Function Invocation**: ```functionName();```

# Operators and Loops

## Operators

* Comparison Operators
* Logical Operators

## Comparison Operators

**Comparison Operators** compare a value in the script to what you might expect. The result will always be a **Boolean** (True/False).

### Types of Comparison Operators

* `==` = is equal to ("soft equal")
* `===` = is strict equal to ("strict equal")
* `!=` = is not equal to
* `!==` = is strict not equal to
* `>` = greater than
* `<` = less than
* `>=` = greater than or equal to
* `<=` = less than or equal to

**Structure of Comparison Operators:**

`(score >= pass)` (must have enclosing parentheses)

This is an **expression**, because it resolves into a *single value* of TRUE or FALSE.

## Logical Operators

**Logical Operators** usually return single values of TRUE or FALSE. They can compare the results of multiple operators.

## Loops

* **Loops** check a **condition**
* If TRUE, a code block runs, and then checks again
* If *still* TRUE, the code block runs again
* Loops will repeat until the condition returns FALSE

### Common Loop Types

* **For Loop**: Used to run code a **specific number of times**
    * Most common loop
    * Condition: Generally a counter telling it how many times to run
    * Good for using a known number of "things"

* **While Loop**: Used if you don't know how many times the code should run
    * Condition: Can be something other than a counter
    * Code will continue to loop as long as condition is TRUE
    * Good for an unknown number of "things"

### Loop Counters

* **Intitialization**: `var i = 0`
    * Create a variable and set it to 0
    * Commonly called '`i`', which acts as the counter
    * Created the first time the loop is run
    * Sometimes '`i`' is declared *before* the function

* **Condition**: `i < 10`
    * Loop should continue running until counter reaches a specific number
    * In `i < 10`, loop will run 10 times before stopping
    * May also hold a variable that in turn holds a number

* **Update**: `i = i + 1` OR `i++`
    * Every time the loop runs the statement in `{ }`, one is added to the counter
    * One is added to the counter with the increment `++` operator
    * Can also count downward using decrement `--` operator

### Assorted Notes

* When you use the `prompt` command, it evaluates *everything entered* as a **string**

Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
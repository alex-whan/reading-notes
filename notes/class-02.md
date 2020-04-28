# Reading 2: HTML Text, CSS Introduction, and Basic JavaScript Instructions

## Selected notes from readings in *HTML & CSS* by Jon Duckett

### Chapter 2 - Text

**Tags** known as **"markup"** provide meaning to a webpage and allow browsers to appropriately display a page's structure
* Structural markup: elements like *headings* and *paragraphs*
* Semantic markup: elements that provide extra information (like where to place emphasis in a sentence, indicating a quotation, etc)

#### Examples of Common Structural Markup

* Headings: `<h1><h2><h3><h4><h5><h6>`
* Paragraphs: `<p>`
* Bold text: `<b>`
* Italic text: `<i>`
* Superscript and Subscript: `<sup>` and `<sub>`

#### Examples of Common Semantic Markup

* Strong and Emphasis: `<strong>` and `<em>`
* Quotations: `<blockquote>` and `<q>`
* Abbreviations and Acronyms: `<abbr>`

### Chapter 10 - Introducing CSS

#### Key Concepts
* CSS stands for "Cascading Style Sheets"
* CSS controls how the content of an element should appear on a page (color, font, etc)
* Associates rules with different HTML elements
* CSS treats each element as if it appears inside its own "box"
* Rules are made of selectors and declarations - and different selectors allow us to target different specific elements

#### Major CSS Selectors

* Universal selector: applies to all elements in a document
* Type selector: matches element names
* Class selector: matches an element identified with the class attribute following the period (.) symbol
* ID selector: matches an element with an "id" attribute, identified with the (#) symbol

#### Specificity in CSS

* Last rule: If there are multiple rules that apply to one element, the last one will take precedence
* Specificity: The more *specific* rule will take precedence over more general ones (i.e., ID `#intro` is more specific than `<h1>`
* Important: A `!` symbol indicates that a property is more important than other rules applied to the same element


## Selected notes from readings in *JavaScript & JQuery* by Jon Duckett

### Chapter 2 - Basic Javascript Instructions

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

### Arrays

**Arrays** are special types of variabes that can store a list of different values (rather than just one value).

* Arrays are useful when working with lists or a set of related values, as you do not need to specify how many items a list will have.

* Arrays are created and named just like regular variables, and then values are assigned to the array inside brackets `[]` and separate by commas

* Values do *not* need to be of the same data type - can be a mix of numbers, strings, and Booleans within the same array

* The "array literal" is constructed as the example below, and is the preferred method for creating them:

`var colors;`
`colors = ['white', 'black', 'custom'];`
`var el = document.getElementByID('colors');`
`el.textContent = colors[0];`

* Note: Arrays start at "0" - so the first value in an array will be [0].

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


### Chapter 4 - Decisions & Loops

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

### Types of Comparison Operators

* `&&` = logical "and"
* `||` = logical "or"
* `!` = logical "not"

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


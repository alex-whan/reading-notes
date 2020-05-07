# Reading 9: Forms and Events

## Selected notes from readings in *HTML & CSS* by Jon Duckett

### Chapter 7 - Forms

### Forms

* **Forms** are used to collect information from visitors to your site

* Form elements use the `<form>` tag

* Information from a form is sent in **name/value pairs**

* User text or value selections in forms are sent to the server 

* Google's homepage/search bar is an ubiquitous example of a form

#### Form controls in HTML5:
* Text input
  - Text input (single-line - email addresses, names)
  - Password input (masks characters entered)
  - Text area (multi-line text input - messages, comments)
* Choosing options
  - Radio buttons (user selects one of multiple options)
  - Checkboxes (user can select/unselect multiple options)
  - Drop-down boxes/menus (user picks an option from a list)
* Submitting forms
  - Submit buttons
  - Image buttons
* Uploading files
  - File upload to a website

#### How Forms Work
1. User fills in a form and presses a button to submit information to server
2. Name of each form control, along with selected/entered user value, is sent to the server
3. Server processesd information using a back-end language (may store it in a database)
4. Server creates a new page based on information received and returns it to user

### Chapter 14 - Lists, Tables, & Forms

#### CSS Properties for Lists, Tables, and Forms

* **Lists**
  - `list-style-type`
  - `list-style-image`
  - `list-style-position`
  - `list-style`

* **Tables**
  - `width`
  - `padding`
  - `text-transform`
  - `letter-spacing`
  - `border-top`, `border-bottom`
  - `text-align`
  - `:hover`
  - `empty-cells: show, hide, inherit`
  - `border-spacing`
  - `border-collapse`

  * **Forms**
    - `font-size`
    - `border, border-radius`
    - `:focus`
    - `:hover`
    - `background-image`
    - `text-shadow`
    - `cursor` - multiple styles for styling cursor in forms



## Selected notes from readings in *JavaScript & JQuery* by Jon Duckett

### Chapter 6 - Events

**Events** are a browser's way of indicating when something has happened (i.e., when a button is clicked or a page finishes loading)

* Events are **fired** or **raised** when they have occured (i.e., a link is tapped or clicked)
* Events **trigger** functions or scripts (i.e., enlarges selected item)

**Binding** indicates which event on a specific node will trigger a response

#### Events & Triggering JavaScript Code

The below steps represent **event handling**:

1. Select the element nodes for the script to respond to
2. Indicate which event on selected nodes will trigger response
3. State code to be run when event occurs

**Event handling** when using a form:

1. Select element: Text input users are interacting with
2. Specify event: When users move out of text input box, it blurs
3. Call code: When "blur" happens, it calls a function (i.e. `checkUserName()`) - and returns an error message if username is too short

#### Event Types
* **UI events:** Occur when a user interacts with browser UI instead of web page
* **Keyboard events:** Occur when a user interacts with keyboard (input event)
* **Mouse events:** Occur when a user interacts with a mouse/touchscreen/touchpad
* **Focus events:** Occur when an element gains or loses focus
* **Form events:** Occur when a user interacts with a form element
* **Mutation events:** Occur when the DOM structre has been altered by a script

#### How to Bind an Event to an Element

* **HTML Event Handlers**
  - Don't use this - bad practice - but you may see it)
* **Traditional DOM Event Handlers**
  - Supported in all major browsers
  - Can only attach a single function to any event
* **Event Listeners (DOM Level 2)**
  - Event listeners are now the preferred standard/modern way of handling elements
  - Allow one event to trigger multiple functions

  #### Example of an Event Listener

  * Below syntax will **bind** and event to an element with an event listener:

    - ```element.addEventListener('event', functionName, [, Boolean]);```

  * Full example:

          ``` function checkUsername(){
            // code to check the length of username
          }
          var el = document.getElementById('username');
          el.addEventListener('blur', checkUsername, false);
          ```
          

Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
# Reading 6: JS Object Literals; The DOM

## Selected notes from readings in *HTML & CSS* by Jon Duckett

### Chapter 3 - Object Literals

#### Objects

**Objects** group together a set of variables and functions to create a model of something you'd recognize from the real world

#### Variables and Functions take on new names within an object:
  
* Variables become known as **properties**
  - Tell us about an object
  - Example: a hotel's name, or the number of rooms it has

* Functions become known as **methods**
  - Represent tasks that are associated with the object
  - Example: checking how many rooms are available at a hotel by subtracting number of booked rooms from number of total rooms

  #### Example of a basic object:

* Object: Hotel
  - Object is in curly braces and is *stored* within a variable called *hotel*
  
  `var hotel = {`
    `name: 'Quay',`
    `rooms: 40,`
    `booked: 25,`
    `gym: true,`
    `roomTypes: ['twin', 'double', 'suite'],`
    `checkAvailability: function () {`
      `return this.rooms - this.booked;`
    `}`
  `}`

  - *"this"* indicates that the function is using the rooms/booked properties of this object (hotel)
  - Properties and methods have **names** and **values**
  - Names in objects are known as **keys**
  - Objects cannot have two keys with the same name
  - Values can be strings, numbers, Booleans, arrays, or another object
  - Method values are *always* functions

  * The combinations of keys and values are called **key/value pairs**

  #### Literal Notation

  * **Literal Notation** is the easiest way to **create** objects
    - Object stored in variable
    - Contents are in curly braces (see above code block)
    - Each key separated from its value by a colon `:`
    - Each property and method separated by a comma `,` - except after the last value

  #### Dot Notation
  
  * You can access properties/methods of an object with **Dot Notation**
    - Alternatively, you can use brackets `[]` to access properties
  * Use the name of the object, followed by a period, then the name of the property/method to be accessed
  * The period `.` is known as the **member operator**

  `var hotelName = hotel.name;`
  `var roomsFree = hotel.checkAvailability();`

  * Alternatively, brackets are used when the name of the property/method contains a special character/number, or when a variable is used in place of the property name:

  `var hotelName = hotel ['name'];`
  `var roomsFree = hotel['checkAvailability']();`


### Chapter 5 - Document Object Model (DOM)

* The **DOM Tree** is a representation of a page in the browser
  - Specifies how browsers should make an HTML model of a page
  - Specifies how JavaScript can access/update the contents while in the browser window
  - The DOM is not part of HTML or JS - it's a *set of rules* implemented by the makers of major browsers

* Two primary areas/abilities of the DOM:
  - Making a model of the HTML page
  - Accessing and changing the HTML page

* DOM = Document Object Model
  - Made up of objects
  - Each object is a different part of the page loaded in browser window

* The DOM is an example of an **Application Programming Interface (API)**
  - APIs let programs/scripts communicate with one another
  - The DOM handles communications between the browsers and the script

* **DOM trees** have four different **node** types:
  - **Document node**: Represents entire page (and corresponds to `document` object)
  - **Element node**: HTML elements
  - **Attribute node**: Attributes of HTML elements - but rather than being children of their parent element, they are *part* of them in the DOM
  - **Text node**: Text within the element node - cannot have children, and is always a new branch of the DOM tree

Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
# Reading 2: Classes, Inheritance, Functional Programming

## Reading, Research, and Discussion

**1. Name 3 advantages to Test Driven Development.**

**2. In what case would you need to use `beforeEach()` or `afterEach()` in a test suite?**

**3. What is one downside of Test Driven Development?**

**4. What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?**

**5. Name a use case for a static method**

**6. Write an example of a Higher Order function and describe the use case it solves**

## Vocabulary Terms

- `functional programming`: A programming paradigm of creating applications and software based on creating pure functions (thereby avoiding shared state, mutable data, and side effects). Declarative rather than imperative. Application state flows through pure functions. [Source](https://medium.com/javascript-scene/master-the-javascript-interview-what-is-functional-programming-7f218c68b3a0).

- `pure function`: A function that always returns the same outputs given the same inputs, with no side effects (such as any work not related to evaluating the actual inputs). [Source](https://www.freecodecamp.org/news/what-is-a-pure-function-in-javascript-acb887375dfe/).

- `higher-order function`: A function that operates based on other functions - that is, taking them in as arguments or returning them. The functions used in the higher-order function can be treated as any other piece of data. [Source](https://eloquentjavascript.net/05_higher_order.html).

- `immutable state`: A state in which values, structures, or data cannot be changed. Means that a certain value or piece of data in a variable can serve as a "source of truth", as it cannot change. Used heavily with React states. [Source](https://css-tricks.com/understanding-immutability-in-javascript/).

- `object`: A representation of a real-life item or person that has properties and methods representing its features and abilities. A dynamic "bag" of properties in JavaScript that in turn is linked to a protype object and its successive chain of prototypes. Can have [Source](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain).

- `object-oriented programming (OOP)`: A programming paradigm of creating applications and software based on using objects to store data in the form of attributes and properties, and code in the form of methods. Programs in OOP act as objects that interact with each other. [Source]().

- `class`: Special functions that are templates for creating objects in JavaScript. Built on prototypes, and encapsulate data with related code needed to work on that data. [Source](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes).

- `prototype`: A special, private property of all JavaScript functions that rests at the top of a inheritance chain, which links to a separate object called a "prototype". This property can be accessed to add new properties or methods to object constructors. [Source](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain).

- `super`: Syntax used to call a parent class constructor when creating an object derived from a parent class. Super syntax explicitly includes the parent constructor properties and methods in the new object constructor. [Source](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes/constructor).

- `inheritance`: All JavaScript objects inherit properties and methods from a prototype, which passes them down a prototype chain. [Source](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain).

- `constructor`: A special method of class used to create and initialize and object instance of that class. Allows for custom initialization of an object.[Source]https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes/constructor).

- `instance`: A new instantiation of an object, called via a function by using the operator `new`. [Source](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Inheritance_and_the_prototype_chain).

- `context`: The object to which a function belongs. The contextual "this" refers to the object in which "this" is used. [Source](https://towardsdatascience.com/javascript-context-this-keyword-9a78a19d5786).

- `this`: A contextual "this" that references the execution context of a function - global context (the global object), function context (inside of a function), class context (inside of a class). Can be a reference to any value in strict mode. [Source](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/this).

- `Test Driven Development (TDD)`: A technique that essentially checks to see if your code functions as expected with the purpose of catching programming errors. Involves defining expected output for production code, and testing to see if the two approaches match. [Source](http://www.letscodejavascript.com/).

- `Jest`: A simple JavaScript testing framework designed to work with Babel, Typescript, Node, React, Angular, Vue, and other libraries. Creates, runs, and structures tests. [Source](https://jestjs.io/en/).

- `Continuous Integration (CI)`: A practice of DevOps software development involving regular merges of new and altered code into a central repository, which then automatically runs tests, builds, and deployments. Helps to detect and correct bugs and issues sooner, reduce development time, and improve overall quality of software. [Source](https://aws.amazon.com/devops/continuous-integration/).

- `unit test`: A test that only tests a single part of the program's implementation (i.e., a single "unit" of the program). Does not test any dependencies or framework specifics. [Source](https://www.freecodecamp.org/news/how-to-start-unit-testing-javascript/).

### Other Sources

- [Medium](https://medium.com/@stevenpcurtis.sc/test-driven-development-tdd-the-advantages-and-disadvantages-5347899ead90)

Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)

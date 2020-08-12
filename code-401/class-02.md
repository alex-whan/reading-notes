# Reading 2: Classes, Inheritance, Functional Programming

## Reading, Research, and Discussion

**1. Name 3 advantages to Test Driven Development.**

- Writing tests prior to the code itself means developers must understand and plan the code's behavior/specifications before it's written.

- Continual testing and refactoring of code increases overall code quality and helps to catch bugs/issues early on in development ('fail fast method').

- Encourages codebase modularity, making for more readable, maintainable, and testable production code.

**2. In what case would you need to use `beforeEach()` or `afterEach()` in a test suite?**

- `beforeEach()`: Runs once _before_ each test case (code block)

- `afterEach()`: Runs once _after_ each test case (code block)

**3. What is one downside of Test Driven Development?**

Writing tests prior to the code itself being written means that developers need to know all of the specifications, features, and requirements of a program before, which can lengthen the early development stages. Benefits of TDD aren't often seen until maintenance phases, and due to the processes involved TDD requires company-wide commitment in order to succeed.

**4. What’s the primary difference between ES6 Classes and Constructor/Prototype Classes?**

The primary difference between ES6 Classes and Constructor/Prototype Classes is that ES6 Classes can define a type of object that is instantiated later on at runtime, while a Constructor/Prototype Class is tied to an actual instance of an object.

**5. Name a use case for a static method**

A common use case for a static method would be a utility function within an application, as static methods do not have access to data stored in specific objects. They could also be used to provide methods to a specific class. Contextual "this" in static methods references the class.

**6. Write an example of a Higher Order function and describe the use case it solves**

      getName = (user) => user.name;
        for (let i=0; i<users.length; i++) {
        const name = getName(users[i]);
      }

**Higher-Order Function**

      usernames = users.map(getName);

This function creates an array of just the users' names, given an array of users. JavaScript's .map() array method is a higher-order function that takes in the getName() function as a parameter.

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

- [Medium - Test Driven Development](https://medium.com/@stevenpcurtis.sc/test-driven-development-tdd-the-advantages-and-disadvantages-5347899ead90)

- [Medium - Static Methods in ES6](https://medium.com/@yyang0903/static-objects-static-methods-in-es6-1c026dbb8bb1#:~:text=Static%20methods%2C%20like%20many%20other%20features%20introduced%20in%20ES6%2C%20are,object%2Doriented%20programming%20in%20Javascript.&text=Static%20methods%20are%20often%20used,data%20stored%20in%20specific%20objects.)

- [FreeCodeCamp - Higher-Order Functions in JS](https://www.freecodecamp.org/news/a-quick-intro-to-higher-order-functions-in-javascript-1a014f89c6b/)

- [Let's Code JavaScript](http://www.letscodejavascript.com/)

- [Mocha Guide to Testing](https://gist.github.com/samwize/8877226)

Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)

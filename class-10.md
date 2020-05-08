# Reading 10: JS Debugging

## Selected notes from readings in *JavaScript & JQuery* by Jon Duckett

### Chapter 10 - Error Handling & Debugging

#### Order of Execution and Execution Contexts

* JavaScript uses three **execution contexts** to interpret code/scripts:
  - **Global execution context**: Code in the script, but not in a function (only one global context per page)
  - **Function context**: Code being run within a function (each function has its own context)
  - **Eval context**: Text is evaluated like code in an internal function called `eval()`

#### Scope

* **Scope** determines where code can run based on its location in the code itself
  - **Global scope**: Defined outside of a function, and can be used anywhere
  - **Function-level scope**: Defined inside of a function, and can only be used within that function
  - **Lexical scope**: Functions defined inside of an object - linked to the object they were defined within

#### The Stack

* JS processes one line of code at a time, and when a statement needs data from another function, it **stacks** that new function on top of the current task
  - When a statement has to call other code, that new task goes to the top of the stack
  - When finished, the JS interpreter returns to the task it was doing before
  - Each new stack item creates a new execution context

#### Hoisting

* Scripts have *two* phases of each new execution context:
  1. Prepare
    - Create new scope
    - Create functions and arguments
  2. Execute
    - Assign values to variables
    - Reference and run functions
    - Execute statements
  
* **Hoisting** is the concept that variables, functions, and arguments can be "used" before they're "created" in the script:

  - Functions can be called before they have been declared if they were created with function expressions

  - Variables can also be assigned values before they're declared

  - Any variables/functions within each execution context are created *before* they are executed - **hoisting** them to the top of the context

  - Each execution context creates its own **variables object**


Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
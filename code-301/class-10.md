# Reading 10: The Call Stack and Debugging

### The Call Stack on MDN

**Call Stack:** A mechanism for a code interpreter (like JavaScript in a web browser) to keep track of its place in a script that calls multiple functions

* Call stack also tracks:
    - What function is currently running
    - What functions are called from within that function

* Basic functionality:
    - When a function is called in a script, the interpreter adds it to the call stack and begins carrying out that function
    - Any functions called by that function are adding to the call stack on *top* of the previous function, and run when the interpreter reaches their calls
    - When current function finishes, interpreter removes it from the top of the stack, and starts executing from wherever it left off in the previous function

* Call stack operates on a **Last In/First Out (LIFO)** format
    - The code lower in the stack cannot be dealt with until the code above it in the stack is executed
    - The last function that gets pushed into the stack is the first to come out when the function returns

* **Stack Overflow:** An error that comes when a stack takes up more space than it had assigned to it

### Understanding the JavaScript Call Stack

#### Call Stack Key Concepts:

* It's **single-threaded** - can only do one thing at a time

* Code execution is **synchronous**

* Function invocations create **stack frames** that occupy temporary memory

* Works in a **Last In/First Out (LIFO) data structure**

### JavaScript Error Messages & Reference

#### Types of Error Messages:

* **Reference Errors:** Occur when you try to use a variable that is not yet declared (or is stuck in the *Temporal Dead Zone* during hoisting)

* **Syntax Errors:** Occur when you have something that cannot be parsed in terms of syntax (like using JSON.parse on an invalid object)

* **Range Errors:** Occur when an object with length is manipulated and given an invalid length (like a negative length for an array)

* **Type Errors:** Occur when the types (number, string, etc) you are trying to use or access are incompatible (like accessing a property in an *undefined* type of variable)
    - Probably the **most frequent error** in JavaScript

Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
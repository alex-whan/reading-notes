# Reading 9: Refactoring & Functional Programming

### Functional Programming Concepts

* **Complexity:** *"Anything that makes software hard to understand or to modify."*

#### What is Functional Programming?

**Functional Programming** is a style of building structure/elements of computer programs that treats computation as the evaluation of mathematical functions and avoids changing-state/mutable data


#### Key Concepts of Functional Programming

##### Pure Functions

**Pure Function:** A *pure function* is when a function:
  - Returns the same result if given the same arguments (deterministic)
  - It does not cause any observable side-effects (like modifying a global object or parameter passed by reference)

* Benefits of pure functions:
  - Code is easier to test (more contexts)

**Functions CANNOT be pure if...**

  - If a function reads external files (file contents can change)
  - If a function relies on a random number generator 

#### Reduce / .reduce()

* **.reduce()** is a key way of making JS code more efficient:
  - Built in JS method
  - **Reduce** receives a **function** and a **collection**, and then returns a value by combining them

* Example: We want the total amount of all books in our shopping cart, laid out as follows:

      let shoppingCart = [
        { productTitle: "Functional Programming", type: "books", amount: 10 },
        { productTitle: "Kindle", type: "eletronics", amount: 30 },
        { productTitle: "Shoes", type: "fashion", amount: 20 },
        { productTitle: "Clean Code", type: "books", amount: 60 }
      ]

**Algorithm** for solving the above with **.reduce()**:

  - **Filter** by book type
  - Transform the shopping cart into a *collection* of amount using **map**
  - Combine all items by adding them up with **reduce**

      
            let shoppingCart = [
              { productTitle: "Functional Programming", type: "books", amount: 10 },
              { productTitle: "Kindle", type: "eletronics", amount: 30 },
              { productTitle: "Shoes", type: "fashion", amount: 20 },
              { productTitle: "Clean Code", type: "books", amount: 60 }
            ]

            const byBooks = (order) => order.type == "books";
            const getAmount = (order) => order.amount;
            const sumAmount = (acc, amount) => acc + amount;

            function getTotalAmount(shoppingCart) {
              return shoppingCart
                .filter(byBooks)
                .map(getAmount)
                .reduce(sumAmount, 0);
            }

            getTotalAmount(shoppingCart); // 70 

* Very useful function!

### Refactoring Javascript for Readability

* **Good code** = Finding the "middle ground" between *speed* and *comprehension* 
  - We want our code to be efficient, but also human-readable and manintainable

  #### Strategies for Refactoring and Reducing Code

  * Return early from functions

  * Cache variables so functions can be read like sentences

  * Check for **Web APIs** before implementing your own functionality

  #### Key Concepts

  * Keep in mind: There will *always* be **edge cases** - sooner or later something will break your code

  * It's often tough to go back and refactor code when working for a company - as once it's functioning, it becomes difficult to convince them changes are needed for the future
    - Better to get things right the first time



Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
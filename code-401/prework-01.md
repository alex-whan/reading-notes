# Prework 1: How to Solve Programming Problems

**Resist the urge to start writing code as soon as possible!**

### Steps for Solving Algorithm-type Programming Problems:

1. Read the problem completely twice
2. Solve the problem manually with 3 sets of sample data
3. Optimize the manual steps
4. Write the manual steps as comments or pseudo-code
5. Replace the comments or pseudo-code with real code
6. Optimize the real code

- NOTE: As much as **70% of your time** should go to **Steps 1-3**

### Detailed Breakdown

#### 1. Read the problem completely twice

- Single most important step - make sure you completely understand the problem
- Make sure you "could explain the problem to someone else"
- If given examples with the problem, make sure you fully work through each one and understand _why_ it works

#### 2. Solve the problem manually

- Solve problem with at least three different inputs to make sure you actually understand the solution for more than one case

  - i.e., Solve for 1, then for 2, and then for _n_

          Example: Reversing a string
          Let’s look at a very basic example, reversing a string.

          If I give you a string “Zebra”, and ask you to reverse it, most people will do the following manual steps.

          Write “Zebra” down.
          Start a new word, and put “a” as the first letter.  (Why –> because it is the last letter, we want to start here)
          Put “r” down as the 2nd letter.  (Why –> because it is the next letter backwards from the last letter we copied)
          Put “b” down as the 3rd letter.  (Why –> same as above)
          Etc

#### 3. Optimize the manual steps

- Very valuable step - optimization is easier in your head than in actual code
- Try to simplify the solution _before_ you code, if possible
- i.e., in the above example, you can write a loop to reduce the manual steps:

            Example: Reversing a string
            Write “Zebra” down.
            Start at the last letter in the word and create a new empty word.
            Append the current letter to the new word
            If there is a previous letter, make the previous letter the current letter and start back at 3.

#### 4. Write the manual steps as comments or pseudo-code

- Especially important step for beginners - helps you get a better grip on all of the steps
- Put them into your text editor as **comments**, or write them as **pseudo-code** that we can translate to real code
- This way, you know exactly what the structure is of the code you'll write - making the actual writing of the code later on simple

        Example: Reversing a string
        // NewWord = “”
        // Loop backwards through word to reverse
        //   NewWord += CurrentLetter
        // Return NewWord

- Outlines code structure

#### 5. Replace the comments or pseudo-code with real code

- At this point, the previous steps will have made this one very simple - no problem solving involved
- Take each comment and convert it into a real line of code
- If you're struggling, consider these reasons:

  - Need to break down the problem into even smaller steps
  - Don't know the programming language well enough to make the conversion

- Write out every single step
- IF you don't know the language well enough, brush up on basic features

- NOTE: For _any_ programming language you expect to be able to work/solve **algorithm type problems** in, you'll need to know how to do the following:
  - Create a list
  - Sort a list or array
  - Create a map or dictionary
  - Loop through a list or dictionary
  - Parse strings
  - Convert from string to int, int to string, etc
- If you don't know how to do _all_ of these things - **stop now and learn them!**

#### 6. Optimize the real code

- Not always necessary, but worth looking at where you can shorten code and take out a few lines if possible
- Ensure that variables are **human-readable** - with long and meaningful names (so that the reviewer can actually understand what you were going for)
- You don't have to get overly complicated with this - just keep your code simple and get rid of duplication (**D.R.Y.**)

### Key Concepts

- Spend 70% of your time thinking about the problem - not writing code
- **"Divide and Conquer"** is an effective method for breaking down problems

Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)

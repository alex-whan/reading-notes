# Reading 26: Component-Based UI

## Review, Research, and Discussion

**1. Name 5 JavaScript UI Frameworks (other than React).**

- Angular
- Vue
- Svelte
- Bootstrap
- Ember

**2. What's the difference between a framework and a library?**

A key difference between a library and a framework is that when using a library, you're in ostensible "control" of the code, whereas with a framework, the framework itself is ultimately in control of the flow of the code itself.

A `library` is essentially a collection of functions and class definitions, packaged together to keep code DRY-er and reduce the need to re-implement algorithms and such. Libraries are also generally more specific in their domains and uses - and aren't necessarily a solution to an entire application.

`Frameworks` are more complex - with their own data and code flows. Rather than requiring you to do the "work" of implementation, you essentially just fill in the "blank spaces" of the framework, and the framework will then call upon that data and content when needed. Think of it like a "skeleton" that you flesh out, but without changing the underlying structure. Developers also do not need to worry about the overall design of a framework working properly.

## Vocabulary Terms

- `rendering`: The process of telling React what to actually display on the screen (tells it to display the specified HTML code inside the specified HTML element). [Source](https://www.w3schools.com/react/react_render.asp).

- `templates`: Methods of separating HTML structures from their content. Basically, they allow you to "plug-and-play" your content without having to worry about writing as much HTML layout code.
  [Source](https://www.sitepoint.com/overview-javascript-templating-engines/).

- `state`: A built-in object of React components that stores property values belonging to said component. When state changes, it triggers a re-render of the component.State should not be modified directly as it can cause strange and unpredictable behavior. [Source](https://www.w3schools.com/react/react_state.asp).

### Other Sources

- [SitePoint: 6 Top JavaScript UI Frameworks & Libraries for 2020](https://www.sitepoint.com/javascript-ui-frameworks/)

- [React Docs - Hello World](https://reactjs.org/docs/hello-world.html)

- [FreeCodeCamp - The Difference Between a Framework and a Library](https://www.freecodecamp.org/news/the-difference-between-a-framework-and-a-library-bd133054023f/)

Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)

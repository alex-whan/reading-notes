# Reading 6: Node, Express, and APIs

### NODE.JS

#### What Is Node.js?

**Node.js** is a JavaScript runtime we can use to execute JavaScript on our computers. 
  - **Important:** Node.js lets us run JavaScript on the server (basically, allows you to write regular JavaScript on the back end)
  - Node is **event-driven**, meaning anything that happens in Node is in reaction to an event (like a request, or an operation finishing)

* Built on Google Chrome's V8 engine 

* I/O = input/output (the communication between a computer/processing system and the outside world/user)


#### Installing Node.js

* `npm` - **"Node Package Manager"** is a package manager that comes bundled with Node
  - `npm -v`: Checks which version you have installed

* **NPM** is also the world's largest **software registry**
  - More than one million packages of JavaScript code available for easy download

* Packages can be installed locally or globally:
  - Global: `npm install -g PACKAGE`
  - Local: `npm init`

* Creating a `package.json` file will allow you to indicate **dependencies** for a certain project (i.e., the packages a project needs to utilize/run)
  - This allows any developer to clone the project and use `npm` to install whatever dependences/packages are needed to run it

#### Using Node.js

* Node automates the process of developing a modern JavaScript application

* Any modern JavaScript framework (i.e. React, Angular, etc.) will need a working knowledge of Node and `npm`
  - Reasoning: These frameworks and many related packages are all available via `npm` and rely on Node to create a dev environment to run in

#### Node.js Execution Model

* Node is **single-threaded** - making it more efficient (traditional servers spawn multiple threads for new requests, which can cause them to become sluggish or crash)

* Node's execution model causes much less overhead to a server and can therefore handle a large number of simultaneous connections
  - Approach to scaling: Clone Node and have the cloned instances share the workload


#### Advantages of Node.js

* Node is well-suited for applications that require real-time interaction or collaboration
  - i.e.: Chat sites, live document editing, APIs receiving lots of request (like database operations), data streaming

* Node makes it possible to process files while they're still being uploaded

* Node has a significant "real-time aspect"

* Great speed and scalability, 

* Ability to use JavaScript on the server side - no translation necessary
  - Everything can be done in the same language and code can easily be shared between server/client

* Node speaks in "JSON" - data can easily flow between layers without reformatting (one syntax all the way through the browser-server-database cycle)

* Excellent support for modern JavaScript (ES6) and beyond - don't have to worry about browser compatibility/breaking code between browsers

#### Downsides of Node.js

* Node does not handle CPU-intensive operations well - these should be handed off to a "worker thread"
  - Overloads can crash the entire process

* Asynchronous coding in JavaScript can be tricky (lots of callbacks)


Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
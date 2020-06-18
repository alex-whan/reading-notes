# Reading 13: Update/Delete

### Sending Form Data

#### METHODS

* **GET:** The GET method is used by the browser to ask a server to send back a resource
  - Browser sends an empty body, which means the data from a form will be appended to the URL in the server

* **POST:** The POST method is the method the browser uses to talk to the server when asking for a response
  - This method takes into account the data provided in the body of the HTTP request
  - If a form is sent with this method, the data is appended to the HTTP request body

* Data must be retrieved on the server side - different methods depend on the development platform:
  - PHP
  - Python
  - Node.js
  - Ruby

* **Frameworks** for the above technologies make handling forms easier:
  - Laravel (PHP)
  - Django (Python)
  - Express (Node.js)
  - Ruby on Rails (Ruby)

#### Security Issues

* "*Be paranoid: Never trust your users*"

* **All** data that comes to your server must be checked and **sanitized** every single time with no exceptions:
  - Escape potentially dangerous characters (like executable code in JS or SQL commands)
  - Limit incoming amount of data to what's necessary
  - Sandbox uploaded files (store them on a different server and control access through a different domain/subdomain)

* Sending form data is easy - securing an application is tougher
  - Front-end developers should not define the security model of data
  - Client-side form validation is possible, but servers cannot/should not trust that validation (no way to verify)

Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
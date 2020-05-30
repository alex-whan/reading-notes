# Reading 13: Local Storage

### The Past, Present, & Future of Local Storage for Web Applications

#### Local Storage

* HTML5's **web storage** is a way for web pages to store *named key/value pairs **locally*** within the browser
  - Similar to **cookies**, as the data persists even after you navigate away from the site, close the browser tab, or exit browser
  - Unlike cookies, data is never transmitted to a remote web server unless doing so manually

* HTML5's web storage is implemented natively in web browsers (even IE!) - making it available even in the absence of third-party plugins

#### Using HTML5 Storage

* Based on named **key/value pairs**
  - Store data based on a named **key**, and then retrieve it using that key
  - Named key **is a string (see below)**, but data can be any type supported by JS

* **Important concept**: In HTML5 storage, **all data is stored as strings**, *not* in its original format
  - Need to use `parseInt()` or `parseFloat()` in order to retrieve anything other than a string

* Browser games can use local storage to save games in progress - so they don't reset when refreshing the browser or closing the tab
  - However, if retrieving anything but a string, the data must be coerced into the correct type to be read

#### Key Limitations of HTML5 Web Storage

* Cannot request more storage
* Storage is limited to 5 MB (otherwise you'll get the `QUOTA_EXCEED_ERR`)
* Default in all browsers is 5 MB

Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)


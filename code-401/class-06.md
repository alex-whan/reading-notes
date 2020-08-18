# Reading 6: HTTP and REST

## HTTP

- **HTTP**: **H**yper **T**ext **T**ransfer **P**rotocol

  - **Stateless** request-response application layer protocol
  - Allows for communication between distributed systems
  - Foundation for the world wide web
  - Apps built with HTTP subscribe to the client-server computer model
  - Current version of protocol is **HTTP/1.1**

- **Client-server computer model**:
  - **Server**: A host designed to provide a service
  - **Client**: A host that makes a request to the server
  - HTTP specifies the format of **requests** and **responses** (known as a **request/response pair**) but not the service itself
  - HTTP generally serves these files (along with many others):
    - `.html`
    - `.json`
    - `.xml`
    - images
    - videos
    - binary executables

## HTTP Requests

- **HTTP Requests**: The request message made from the client to the server

- First line of an HTTP Request contains:

  - `METHOD`
  - `URL`
  - `HTTP VERSION`

- Following lines contain:
  - `REQUEST HEADERS`
    - Headers are **key/value pairs** separated by colons
    - Headers with more than one value separate values with a semicolon
    - Each Header is separated by a `newline character`
    - Header section is terminated with an empty line
    - An optional `body` follows the header section

### Example HTTP Request

      POST /api/note HTTP/1.1
      Host: api.example.com
      Origin: www.example.com
      Authorization: Bearer bHVsIHRoaXMgaXMgYSBmYWtlIHNlY3JldCB0b2tlbg==
      Accept: application/json
      Content-Type: application/json; charset=UTF-8
      Content-Length: 58

      {"title":"kata","content":"get 100 points on hacker rank"}

## HTTP Responses

- **HTTP Responses**: The response message from the server to the client

### Example HTTP Reponse

      HTTP/1.1 200 OK
      Date: Tue, 22 Aug 2017 06:34:16 GMT
      Content-Type: application/json; charset=UTF-8
      Content-Encoding: UTF-8
      Content-Length: 82
      Last-Modified: Mon, 21 Aug 2017 12:10:38 GMT
      Server: Apache/1.3.3.7 (Unix) (Red-Hat/Linux)
      ETag: "3f80f-1b6-3e1cb03b"
      Connection: close

      {"id":"1234123412341324","title":"kata","content":"get 100 points on hacker rank"}

## HTTP Methods

| **HTTP Method (Verb)** | **Request has Body** | **Response has Body** | **Safe** | **Idempotent** | **Cachable** |            **Function**             |
| :--------------------: | :------------------: | :-------------------: | :------: | :------------: | :----------: | :---------------------------------: |
|          GET           |          no          |          yes          |   yes    |      yes       |     yes      |         Retrieve a resource         |
|          HEAD          |          no          |          no           |   yes    |      yes       |     yes      |   Like GET - but only for HEADERS   |
|          POST          |         yes          |          yes          |    no    |       no       |     yes      |        Create a new resource        |
|          PUT           |         yes          |          yes          |    no    |      yes       |      no      |          Update a resource          |
|         DELETE         |          no          |          yes          |    no    |      yes       |      no      |          Delete a resource          |
|        CONNECT         |         yes          |          yes          |    no    |       no       |      no      |       Create a TCP/IP tunnel        |
|        OPTIONS         |       optional       |          yes          |   yes    |      yes       |      no      | Returns supported methods for a URL |
|         TRACE          |          no          |          yes          |   yes    |      yes       |      no      |      Echoes retrieved request       |
|         PATCH          |         yes          |          yes          |    no    |       no       |      no      |    Partially modifies a resource    |

- Only methods with `safe` should be used to retrieve information - they should _not_ change the server state
- `Idempotent` methods means that two identical requests should get an indentical response
- `Cahceable` methods mean the client should be able to `cache` the response

## REST

- **REST** = **Re**presentational **S**tate **T**ransfer
  - A means by which we can reference, manipulate, and transfer **state**

## REST Methods

| **REST Method (Verb)** | **CRUD Operation** | **Function**                                   |
| :--------------------: | :----------------: | :--------------------------------------------- |
|          GET           |        READ        | Retrieve 1 or more Records                     |
|          POST          |       CREATE       | Create a New Record                            |
|          PUT           |       UPDATE       | Replace entire Record with an updated version  |
|         PATCH          |       UPDATE       | Replace only the changed portion of the Record |
|        DESTROY         |       DELETE       | Remove a Record                                |

- RESTful **endpoints** generally deliver data in JSON format

  - Best practice: Supply a header with metadata and a collection of results

- REST uses **methods (VERBS)** to operate on the **state** of a **resource (NOUN)**

  - HTTP is generally used as a **transfer protocol**

- **RESTful Endpoint**: A URI that identifies the specific resource
  - We can access these endpoints with a method - which, if used correctly, can affect the state of a resource
  - This means we can **perform CRUD operations over HTTP**

Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)

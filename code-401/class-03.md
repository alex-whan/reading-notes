# Reading 3: Data Modeling & NoSQL Databases

## Reading, Research, and Discussion

**1. Why would a developer choose to make data models?**

**2. What purpose do CRUD operations serve?**

**3. What kind of database is Postgres? What kind of database is MongoDB?**

**Postgres is a Relational Database - which uses SQL.**

Relational (SQL) databases are based off of tables, and represent data as tables with a certain number of columns and rows of data. They use schemas to determine and define how data must be composed when inserted.

**MongoDB is a non-relational or distributed database - which is a non-SQL database (NoSQL).**

Non-Relational (NoSQL) databases are based off of documents, key-value pairs, graphs, wide-column stores, or other irregular data. The database consists of two or more files in different sites, and may be stored across multiple computers or networks.

NoSQL databases are a collection of data (can be in the forms previously listed) that do not have a standard schema definition. They allow for the storage and manipulation of unstructured, semistructured, or irregularly-structured data.

**4. What is Mongoose and why do we need it?**

**5. Define three related pieces of data in a possible application. An example for a store application might be Product, Category and Department. Describe the constraints and rules on each piece of data and how you would relate these pieces to each other. For example, each Product has a Category and belongs in a Department.**

## Vocabulary Terms

- `database`: An organized collection of data/information stored electronically in a computer system, and controlled/accessed via a Database Management System (DBMS).[Source](https://www.oracle.com/database/what-is-database.html).

- `data model`: A data structure that determines how data is organized, as well as how its elements relate to one another. [Source](https://cedar.princeton.edu/understanding-data/what-data-model).

- `CRUD`: An acronym for the four basic SQL commands: Create, Read, Update, and Delete. Each corresponds to an HTTP method. Most modern applications feature some or full CRUD functionality. "CRUD applications" use forms to access information in a database. [Source](https://docs.jboss.org/tools/3.3.0.Final/en/seam_tools_ref_guide/html/crud_database_application.html#:~:text=CRUD%20is%20an%20acronym%20for,and%20out%20of%20a%20database.).

- `schema`: A collection of data structures that determines how data can be inserted into a database. Lays out the structure and organization of a database.[Source](https://database.guide/what-is-a-database-schema/).

- `unit test`: A test that runs in isolation - focusing on a single block of code or individual module. [Source]().

- `sanitize`: The process of checking data to ensure there are no inputs that might make the program vulnerable to attacks (such as a SQL injection attack). Prevents users from entering data directly into a database. [Source]().

- `Structured Query Language (SQL)`: A standard language used to access and manipulate databases through the use of queries and commands. Multiple versions of the language exist, all with standard commands. [Source](https://www.w3schools.com/sql/sql_intro.asp).

- `Non SQL (NoSQL)`: NoSQL databases have dynamic schema for unstructured data. Popular with more complex web applications.[Source](https://www.oracle.com/database/what-is-database.html).

- `MongoDB`: A cross-platform, document-oriented, NoSQL database program (non-relational/distributed database). Utilizes documents with a JSON-style format. Schemas are optional. [Source](https://en.wikipedia.org/wiki/MongoDB).

- `Mongoose`: [Source]().

- `record`: An object representing a group of data saved in a database table. Displays a set of fields related to the object's properties and values (such as an employee ID, name, position, hire date, etc.). [Source](https://teachcomputerscience.com/database-record/).

- `document`: A JSON-like model for storing irregular data in a database. Map to objects in code for a more natural/intuitive flow. [Source](https://www.mongodb.com/document-databases).

- `Object Relation Mapping (ORM)`: [Source]().

### Other Sources

- [The Geek Stuff - SQL vs NoSQL](https://www.thegeekstuff.com/2014/01/sql-vs-nosql-db/?utm_source=tuicool)

- [Database Record](https://teachcomputerscience.com/database-record/)

Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)

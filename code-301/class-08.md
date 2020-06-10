# Reading 8: SQL

### What Is SQL?

**SQL:** Structured Query Language

* Designed to allow technical and non-technical users to **query**, **manipulate**, and **transform** data from a regional **database**

* Provides storage for websites and mobile applications

* Popular SQL databases include:
  - SQLite
  - MySQL
  - Postgres
  - Oracle
  - Microsoft SQL Server

* All databases support common SQL language standard, though implementation in terms of features/storage types can differ between them

#### SQL and Relational Databases

* **Relational database:** A collection of related two-dimensional tables
  - Similar to an Excel spreadsheet: Fixed number of named columns (attributes/properties) + any number of rows of data

### SQL Functionality

#### SELECT Statements (Queries)

* **SELECT Statements** (also known as **queries**) allow us to retrieve data from a SQL database
  - Essentially: 
    - Declares what data we're looking for,
    - Where to find it in the database,
    - How to transform it before it's returned (optional)

* Think of a SQL table as an **entity** (i.e. Cars, Dogs)
  - Think of each table row as an **instance** of that type of thing (i.e. pug, beagle, lab)
  - Columns represent the common properties shared between all instances of that entity (i.e. color of fur, length of tail, etc.)

* Most basic query would be selecting a few columns (properties) of a table with all rows (instances):
          
          SELECT column, another_column, ...
          FROM mytable

* Alternatively, you could retrieve ALL columns of data using an asterisk (*)
  - This is especially useful as you can select a table and dump all of its data at once:

          SELECT *
          FROM mytable;

### SQL Cheat Sheet


Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
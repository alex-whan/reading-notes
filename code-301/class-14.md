# Reading 14: Database Normalization

### Database Normalization Explained in Simple English

#### Key Concepts and Intro to Database Normalization

**Database Normalization:** A process used to organize a database into tables and columns (*redesigning the table*)

* **Key concepts:**
  - Tables should be about specific topics
  - Only supporting topics should be included
  - This limits the table to one purpose and reduces duplicate data in your database
  - Helps cut down on issues stemming from database modifications

**Three main reasons for database normalization:**
  1. Minimize duplicate data
  2. Minimize/avoid data modification issues
  3. Simplify queries

#### Data Duplication and Modification Anomalies

* Data duplication/duplicated information poses a problem because:
  - It increases storage and decreases performance
  - It becomes more difficult to maintain data changes

#### Main Modification Anomalies:

* **Insert Anomaly:** Data that cannot be recorded until all other data for the entire row is also known (i.e., to create a record, we must have the primary key)

* **Update Anomaly:** If we do not update all the rows (especially with duplicate info), inconsistencies appear

* **Deletion Anomaly:** Row deletion can cause removal of more information than intended

* **Search and Sort Issues:** Separating data into different tables serving a single purpose means it's then easier to write *queries* (fewer columns to consider)

#### Definitions of Database Normalization

* Three common **forms** of database normalization
  - These forms are progressive (to qualify for the 2nd normal form, a table must satisfy the rules of the 1st normal form, etc.)
  - 1st, 2nd, and 3rd normal forms are known as **1NF**, **2NF**, and **3NF**, respectively

* Key concept: There are three common rules for database normalization, and they depend upon each other

* **First Normal Form (1NF):** The information is stored in a **relational table** with each column containing atomic values. There are no repeating groups of values.

* **Second Normal Form (2NF):** The table is in first normal form, and all the columns depend on the table's primary key.

* **Third Normal Form (3NF):** The table is in the second normal form, and all of its columns are not transitively dependent on the primary key.

Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)
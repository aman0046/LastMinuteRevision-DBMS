# DBMS Notes - Last Minute Revision :white_check_mark: 

Here we have last minute revision notes of DBMS. These questions will familiarize you with the most important DBMS concepts and help you ace your job interviews :raised_hands:

## Most Asked DBMS Interview Questions

### 1) What is DBMS?
A DBMS is software that manages databases, providing an interface to store, retrieve, and manipulate data efficiently and securely.

---

### 2) What is a Database?
A Database is an organized, consistent, and logical collection of data that can easily be updated, accessed, and managed. Database mostly contains sets of tables or objects which consist of records and fields. 

---

### 2) Explain the difference between a database and a DBMS?
A database is a collection of related data, while a DBMS is software used to manage, store, and retrieve data efficiently from the database.

---

### 3) What is the different languages present in DBMS?

- **DDL(Data Definition Language)**:  It contains commands which are required to define the database. \ 
E.g., CREATE, ALTER, DROP, TRUNCATE, RENAME, etc.
- **DML(Data Manipulation Language)**: It contains commands which are required to manipulate the data present in the database. \
E.g., SELECT, UPDATE, INSERT, DELETE, etc.
- **DCL(Data Control Language)**:  It contains commands which are required to deal with the user permissions and controls of the database system. \
E.g., GRANT and REVOKE.
- **TCL(Transaction Control Language)**:  It contains commands which are required to deal with the transaction of the database. \
E.g., COMMIT, ROLLBACK, and SAVEPOINT.

---

### 4) ACID properties in DBMS?
ACID stands for Atomicity, Consistency, Isolation, and Durability in a DBMS these are those properties that ensure a safe and secure way of sharing data among multiple users.

- **Atomicity**: This property reflects the concept of either executing the whole query or executing nothing at all, which implies that if an update occurs in a database then that update should either be reflected in the whole database or should not be reflected at all.
- **Consistency**: This property ensures that the data remains consistent before and after a transaction in a database.
- **Isolation**: This property ensures that each transaction is occurring independently of the others. This implies that the state of an ongoing transaction doesn’t affect the state of another ongoing transaction.
- **Durability**: This property ensures that the data is not lost in cases of a system failure or restart and is present in the same state as it was before the system failure or restart.

---

### 5) Difference between the DELETE and TRUNCATE command in a DBMS?

- DELETE Command:
    - It removes rows from a table one by one with transaction logging
    - It can be rolled back if required.

- TRUNCATE Command:
    - It removes all rows at once without transaction logging.
    - It can't be rolled back.
 
---

### 6) What is meant by Normalization and Denormalization?

**Normalization** is a process of reducing redundancy by organizing the data into multiple tables. Normalization leads to better usage of disk spaces and makes it easier to maintain the integrity of the database.  

**Denormalization** is the reverse process of normalization as it combines the tables which have been normalized into a single table so that data retrieval becomes faster. JOIN operation allows us to create a denormalized form of the data by reversing the normalization. 


---

### Different types of Normalization forms in a DBMS?

- 1NF: It is known as the first normal form and is the simplest type of normalization that you can implement in a database. A table to be in its first normal form should satisfy the following conditions:
    - Every column must have a single value and should be atomic.
    - Duplicate columns from the same table should be removed.
    - Separate tables should be created for each group of related data and each row should be identified with a unique column.
 
- 2NF: It is known as the second normal form. A table to be in its second normal form should satisfy the following conditions:
    - The table should be in its 1NF i.e. satisfy all the conditions of 1NF.
    - Every non-prime attribute of the table should be fully functionally dependent on the primary key i.e. every non-key attribute should be dependent on the primary key in such a way that if any key element is deleted then even the non_key element will be saved in the database.
 
- 3NF: It is known as the third normal form. A table to be in its third normal form should satisfy the following conditions:
    - The table should be in its 2NF i.e. satisfy all the conditions of 2NF.
    - There is no transitive functional dependency of one attribute on any attribute in the same table.
 
- BCNF: BCNF stands for Boyce-Codd Normal Form and is an advanced form of 3NF. It is also referred to as 3.5NF for the same reason. A table to be in its BCNF normal form should satisfy the following conditions:
    - The table should be in its 3NF i.e. satisfy all the conditions of 3NF.
    - For every functional dependency of any attribute A on B
(A->B), A should be the super key of the table. It simply implies that A can’t be a non-prime attribute if B is a prime attribute.


---


### What is an Entity-Relationship Diagram (ER-Diagram)?  
An ER-Diagram is a visual representation of the relationships among entities in a database, showing how different tables are connected.

---

### Different types of keys in a database?

- **Primary key**: The Primary key is an attribute in a table that can uniquely identify each record in a table. It is compulsory for every table.
- **Unique Key**: The unique key is very similar to the primary key except that primary keys don’t allow NULL values in the column but unique keys allow them.
- **Foreign key**: The Foreign key is a primary key from one table, which has a relationship with another table. It acts as a cross-reference between tables.

---

### What is a lock. Explain the difference between a shared lock and an exclusive lock?

A database lock is a mechanism to protect a shared piece of data from getting updated by two or more database users at the same time. When a single database user or session has acquired a lock then no other database user or session can modify that data until the lock is released.

- **Shared lock**: Shared lock is required for reading a data item. In the shared lock, many transactions may hold a lock on the same data item. When more than one transaction is allowed to read the data items then that is known as the shared lock.

- **Exclusive lock**: When any transaction is about to perform the write operation, then the lock on the data item is an exclusive lock. Because, if we allow more than one transaction then that will lead to the inconsistency in the database.

---

### What are Views in DBMS?

A view is a virtual table that is derived from one or more base tables or other views. It does not store any data itself but represents a tailored, pre-defined query that simplifies data retrieval. Views act as a layer of abstraction over the underlying tables, providing a more user-friendly and secure way to interact with the data.

**Benefits of using views**:

- **Data Abstraction**: Views allow users to work with a simplified representation of the data, hiding unnecessary details and complexity.
- **Security**: Views can be used to restrict access to certain columns or rows, providing a level of security by only showing specific data to specific users.
- **Simplified Querying**: Complex queries can be encapsulated within views, making it easier for users to retrieve the desired information without writing complex SQL statements.
- **Data Independence**: If the underlying schema changes, views can remain the same, and applications using the views will not be affected.

---





















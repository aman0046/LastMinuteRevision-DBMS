# DBMS Notes - Last Minute Revision :white_check_mark: 

Here we have last minute revision notes of DBMS. These questions will familiarize you with the most important DBMS concepts and help you ace your job interviews :raised_hands:

---

###

#### Join us for all the latest offcampus job updates, webinar, hackathons, resume review and a lot more :heart::heart:

<div align="left">
  <a href="https://www.linkedin.com/in/amanchowdhury046/" target="_blank">
    <img src="https://img.shields.io/static/v1?message=LinkedIn&logo=linkedin&label=&color=0077B5&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="linkedin logo"  />
  </a>
  <a href="https://www.youtube.com/@amanchowdhury046" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Youtube&logo=youtube&label=&color=FF0000&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="youtube logo"  />
  </a>
  <a href="https://telegram.me/offcampus_phodenge" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Telegram&logo=telegram&label=&color=2CA5E0&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="telegram logo"  />
  </a>
  <a href="https://www.instagram.com/aman_chowdhury_046/" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Instagram&logo=instagram&label=&color=E4405F&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="instagram logo"  />
  </a>
  <a href="https://whatsapp.com/channel/0029Va9Q0lkDZ4LYNx6ukw2u" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Whatsapp&logo=Whatsapp&label=&color=25D366&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="whatsapp logo"  />
  </a>
</div>

###

---

## Most Asked DBMS Interview Questions

<img src="/assets/images/DBMS.png" width="600" height="200">

### 1) What is DBMS?
A DBMS is software that manages databases, providing an interface to store, retrieve, and manipulate data efficiently and securely.

---

### 2) What is a Database?
A Database is an organized, consistent, and logical collection of data that can easily be updated, accessed, and managed. Database mostly contains sets of tables or objects which consist of records and fields. 

---

### 3) Explain the difference between a database and a DBMS?
A database is a collection of related data, while a DBMS is software used to manage, store, and retrieve data efficiently from the database.

---

### 4) Advantages of DBMS over File Systems?

- **Data Redundancy and Inconsistency**: \
Redundancy means repeating the data in a system. In a normal file system, there is a high chance that there can be various files of the same data used by different users for specific purposes. If any user changes the data in its files, then the changes are not reflected in all files. This creates inconsistency in the data, and it may lead to the failure of the system. But in the DBMS, there is only one repository of data, and multiple users can use it. If any user changes the data, then it is reflected to each user as they are using the same repository.

- **Data Sharing**: \
In the normal file system, data sharing is too difficult because file sharing is a complex task. In DBMS, all the data is centralized, so data sharing is a very easy task.

- **Data Concurrency**: \
When more than one user accesses the database simultaneously, then it is called concurrency. In a file system, when multiple users are using the files at the same time, then there may be a chance of anomalies in the data due to changes, and it does not provide any method to detect anomalies. But in DBMS, we have a locking system to detect the anomalies so we can protect the data.

- **Data Searching**: \
To search the data in a file system, we have to write a specific program and run it. In DBMS, we have query languages by which we can write small queries to get the data we want from the database. We can use various query languages, like MySQL, Oracle, etc., for a database to search and retrieve the data.

- **Data Integrity**: \
When we insert new data into the database, we require some specific constraints on the data like integer or not null, etc. The file system does not provide any system to check the constraints, whereas DBMS has the functionality to check the constraints on the data, and it allows user defined data types.


---

### 5) What is the different languages present in DBMS?

- **DDL(Data Definition Language)**:  It contains commands which are required to define the database. \ 
E.g., CREATE, ALTER, DROP, TRUNCATE, RENAME, etc.
- **DML(Data Manipulation Language)**: It contains commands which are required to manipulate the data present in the database. \
E.g., SELECT, UPDATE, INSERT, DELETE, etc.
- **DCL(Data Control Language)**:  It contains commands which are required to deal with the user permissions and controls of the database system. \
E.g., GRANT and REVOKE.
- **TCL(Transaction Control Language)**:  It contains commands which are required to deal with the transaction of the database. \
E.g., COMMIT, ROLLBACK, and SAVEPOINT.

---

### 6) ACID properties in DBMS?

<img src="/assets/images/ACID.png" width="600" height="200">

ACID stands for Atomicity, Consistency, Isolation, and Durability in a DBMS these are those properties that ensure a safe and secure way of sharing data among multiple users.

- **Atomicity**: This property reflects the concept of either executing the whole query or executing nothing at all, which implies that if an update occurs in a database then that update should either be reflected in the whole database or should not be reflected at all.
- **Consistency**: This property ensures that the data remains consistent before and after a transaction in a database.
- **Isolation**: This property ensures that each transaction is occurring independently of the others. This implies that the state of an ongoing transaction doesn’t affect the state of another ongoing transaction.
- **Durability**: This property ensures that the data is not lost in cases of a system failure or restart and is present in the same state as it was before the system failure or restart.

---

### 7) Difference between the DELETE and TRUNCATE command in a DBMS?

- DELETE Command:
    - It removes rows from a table one by one with transaction logging
    - It can be rolled back if required.

- TRUNCATE Command:
    - It removes all rows at once without transaction logging.
    - It can't be rolled back.
 
---

### 8) What is meant by Normalization and Denormalization?

<img src="/assets/images/D&N.webp" width="600" height="200">

**Normalization** is a process of reducing redundancy by organizing the data into multiple tables. Normalization leads to better usage of disk spaces and makes it easier to maintain the integrity of the database.  

**Denormalization** is the reverse process of normalization as it combines the tables which have been normalized into a single table so that data retrieval becomes faster. JOIN operation allows us to create a denormalized form of the data by reversing the normalization. 


---

### 9) Different types of Normalization forms in a DBMS?

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


### 10) What is an Entity-Relationship Diagram (ER-Diagram)?  
An ER-Diagram is a visual representation of the relationships among entities in a database, showing how different tables are connected.

---

### 11) Different types of keys in a database?

- **Primary key**: The Primary key is an attribute in a table that can uniquely identify each record in a table. It is compulsory for every table.
- **Unique Key**: The unique key is very similar to the primary key except that primary keys don’t allow NULL values in the column but unique keys allow them.
- **Foreign key**: The Foreign key is a primary key from one table, which has a relationship with another table. It acts as a cross-reference between tables.

---

### 12) What is a lock. Explain the difference between a shared lock and an exclusive lock?

A database lock is a mechanism to protect a shared piece of data from getting updated by two or more database users at the same time. When a single database user or session has acquired a lock then no other database user or session can modify that data until the lock is released.

- **Shared lock**: Shared lock is required for reading a data item. In the shared lock, many transactions may hold a lock on the same data item. When more than one transaction is allowed to read the data items then that is known as the shared lock.

- **Exclusive lock**: When any transaction is about to perform the write operation, then the lock on the data item is an exclusive lock. Because, if we allow more than one transaction then that will lead to the inconsistency in the database.

---

### 13) What are Views in DBMS?

A view is a virtual table that is derived from one or more base tables or other views. It does not store any data itself but represents a tailored, pre-defined query that simplifies data retrieval. Views act as a layer of abstraction over the underlying tables, providing a more user-friendly and secure way to interact with the data.

**Benefits of using views**:

- **Data Abstraction**: Views allow users to work with a simplified representation of the data, hiding unnecessary details and complexity.
- **Security**: Views can be used to restrict access to certain columns or rows, providing a level of security by only showing specific data to specific users.
- **Simplified Querying**: Complex queries can be encapsulated within views, making it easier for users to retrieve the desired information without writing complex SQL statements.
- **Data Independence**: If the underlying schema changes, views can remain the same, and applications using the views will not be affected.

---

### 14) What is a Join? List its different types.

The SQL Join clause is used to combine records (rows) from two or more tables in a SQL database based on a related column between the two.

There are four different types of JOINs in SQL:

<img src="/assets/images/JOIN.png" width="600" height="200">

- **INNER JOIN**: Retrieves records that have matching values in both tables involved in the join. This is the widely used join for queries.
- **LEFT OUTER JOIN**: Retrieves all the records/rows from the left and the matched records/rows from the right table.
- **RIGHT OUTER JOIN**: Retrieves all the records/rows from the right and the matched records/rows from the left table.
- **FULL OUTER JOIN**: Retrieves all the records where there is a match in either the left or right table.

---

### 15) What is a Self-Join?
A self JOIN is a case of regular join where a table is joined to itself based on some relation between its own column(s). Self-join uses the INNER JOIN or LEFT JOIN clause and a table alias is used to assign different names to the table within the query.

---

### 16) What is a Cross-Join?
Cross join can be defined as a cartesian product of the two tables included in the join. The table after join contains the same number of rows as in the cross-product of the number of rows in the two tables. If a WHERE clause is used in cross join then the query will work like an INNER JOIN.

---

### 17) What is an Index? Difference between Clustered and Non-Clustered Index?

A database index is a data structure that provides a quick lookup of data in a column or columns of a table. It enhances the speed of operations accessing data from a database table at the cost of additional writes and memory to maintain the index data structure.

#### Difference between Clustered and Non-Clustered Index

- Clustered index modifies the way records are stored in a database based on the indexed column. A non-clustered index creates a separate entity within the table which references the original table.
- Clustered index is used for easy and speedy retrieval of data from the database, whereas, fetching records from the non-clustered index is relatively slower.
- In SQL, a table can have a single clustered index whereas it can have multiple non-clustered indexes.


---



### Thanks for Reading 

<img src="/assets/images/save.png" width="600" height="200">

---

###

#### Join us for all the latest offcampus job updates, webinar, hackathons, resume review and a lot more :heart::heart:

<div align="left">
  <a href="https://www.linkedin.com/in/amanchowdhury046/" target="_blank">
    <img src="https://img.shields.io/static/v1?message=LinkedIn&logo=linkedin&label=&color=0077B5&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="linkedin logo"  />
  </a>
  <a href="https://www.youtube.com/@amanchowdhury046" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Youtube&logo=youtube&label=&color=FF0000&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="youtube logo"  />
  </a>
  <a href="https://telegram.me/offcampus_phodenge" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Telegram&logo=telegram&label=&color=2CA5E0&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="telegram logo"  />
  </a>
  <a href="https://www.instagram.com/aman_chowdhury_046/" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Instagram&logo=instagram&label=&color=E4405F&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="instagram logo"  />
  </a>
  <a href="https://whatsapp.com/channel/0029Va9Q0lkDZ4LYNx6ukw2u" target="_blank">
    <img src="https://img.shields.io/static/v1?message=Whatsapp&logo=Whatsapp&label=&color=25D366&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="whatsapp logo"  />
  </a>
</div>

###

---




















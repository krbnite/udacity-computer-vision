
Objectives
* foundation for database management
* identify features of database management systems and database processing environments
* create tables and formulate business queries using SQL
* create entity relationship diagrams (ERD) to represent business requirements
* convert ERD to a table design
* analyze table designs for unwanted redundancy
* reflect on guidelines for query formulation, redundancy elimination, and data modeling

Will:
* create tables in a relational database and define integrity rules for those tables
* write statemetns in a database language to retrieve data from a relational databse
  - learn how to apply the query formulation process to transform an unstructured problem statement into a database language statement
* learn data modeling
  - notation for entity relationship diagrams
  - use ERDs to represent data requirements for a business situation
* convert ERD to a table design without excessive redundancy

Some Resources:
* [SQL Fiddle](http://sqlfiddle.com/)
  - create table schema, insert data, and run queries
  - supports MySQL, Postgres, and SQLite syntax (and more)
* https://dev.mysql.com/downloads/
  - download MySQL community edition server and client
  

Important characteristics of a database:
* persistency: data lasts longer than the state of computer memory when the computer shuts down
* inter-related:  relationships between entities
* shared: many applications and users need to access the database simultaneously

This course focuses on database for daily operations (transactional).  In other courses in
the sequence, we focus on databases used for business intelligence (datawarehouses). This course
also focuses on conventional structured data (e.g., names, addresses, accounts). 

-------------------

Database Management System (DBMS): a collection of components that supports that creation,
use, and maintenance of databases.

DBMS Features:
* data acquisition
* storage
* dissemination
* maintenance
* retrieval 
  - nonprocedural data access (query language)
  - form tool
  - visual tools
* formatting
  - reporting tool



Types of DBMSs:
* Enterprise DBMS
  - used for organization with very large databases and/or thousands of simultaneous users
  - strong reliability and performance! 
  - Enterprise DBMSs are offered by
    * Oracle
    * MySQL 
    * Microsoft
    * Teradata
* Desktop DBMSs
 - small work groups with small-to-moderate sized databases
 - tens of simultaneous users
 - modest reliability and performance
 - Example: Microsoft Access

Database transactions: a collection of operations that must be reliably processed as one unit
of work; transactions are all or nothing -- all the operations of a transaction must succeed or
the entire transaction is canceled.  A transaction is reliable: there should be no loss of data
due to interference among concurrent users and/or failures, such as OS crashes.

Transaction in pseudocode
```
START TRANSACTION
    Display greeting
    Get reservation preferences from user
    SELECT departure and return flight records
    If reservation is acceptable then
        UPDATE seats remaining of departure flight record
        UPDATE seats remaining of return flight record
        INSERT reservation record
        Email receipt if requested
    EndIf
    OnError: ROLLBACK
COMMIT
```

DBMS features that implement transactionality:
* concurrency control manager
* recovery manager 

Data Warehouse: Refers to a logically centralized data repository where data from operational
databases and other sources are integrated, cleaned, and standardized to support business
intelligence.

Differences between transactional and BI databases:
* Transactional Processing
  - primary data in operational databases
  - large volumes of transactions with small amounts of data
  - some reporting requirements for operations
  - process orientation (e.g., order entry)
  - a transactional query deals with a few records
* Business Intelligence Processing
  - secondary data from operational databases
  - substantial processing for transformations and integration
  - large volumes of data reporting
  - subject orientation (e.g., all order data, all customer data)
  - a BI query deals with thousands or millions of records
  - requires a lot of compute for transformation and integration processes; usually run off peak hours



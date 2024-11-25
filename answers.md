##SQL-Assignment-Week-1

State and Explain the components of a DBMS(Database Management System)
1. Database Engine

    The core service for accessing and processing data. The database engine handles all operations related to data storage, retrieval, and updating. It is responsible for executing queries, managing transactions, and ensuring data consistency and integrity.

2. Database Schema

    The structure that defines how data is organized within the database. It includes the definition of tables, fields, data types, relationships, and constraints. The schema acts as a blueprint for the database, outlining how data is to be stored and accessed.

3. Query Processor

    Interprets and executes database queries. The query processor translates high-level SQL queries into a form that the database engine can understand. It also optimizes query execution to retrieve data efficiently.

4. Database Manager

    Manages the database’s data structure and handles tasks such as data storage, backup, recovery, and access control. The database manager ensures that data is stored securely and can be retrieved or modified as needed.

5. Data Dictionary

    A centralized repository that contains metadata about the database, such as information about tables, columns, data types, and relationships. The data dictionary acts as a reference for users and the system itself to understand the structure and organization of the database.

6. Transaction Management

    Ensures the database maintains its integrity, even in cases of system failures or errors. It handles transactions, which are sequences of operations that must be completed as a unit. The transaction manager ensures that transactions are processed reliably and follow the ACID (Atomicity, Consistency, Isolation, Durability) properties.

7. User Interface (UI)

    The interface through which users interact with the DBMS. This can be in the form of a command-line interface (CLI) for SQL commands or a graphical user interface (GUI) that provides a more user-friendly way to manage databases.

8. Reporting and Data Analysis Tools

    These are tools integrated into the DBMS to generate reports and perform data analysis. They help in extracting meaningful insights from the stored data, which can be used for decision-making purposes.

9. Storage Management

    Manages how data is physically stored in the database. It deals with disk space allocation, indexing, data clustering, and data compression to ensure efficient storage and quick access.


What is a relational database? Give 4 examples.

A relational database is a type of database that organizes data into tables (also known as relations) consisting of rows and columns. Each table represents a specific entity, and the relationships between tables are established using keys, such as primary keys and foreign keys.

                 Examples:
                 MySQL
                 PostgreSQL
                 Oracle Database
                 Microsoft SQL Server
                 

State and Explain three classifications of SQL?

Data Definition Language (DDL)
    DDL statements are used to define, modify, and manage the structure of database objects such as tables, indexes, and schemas. 
    
Data Manipulation Language (DML)
    DML statements are used for managing data within database objects. These commands allow for inserting, updating, deleting, and retrieving data from the database tables.

 Data Control Language (DCL)
     DCL statements are used to control access to data within the database. These commands manage user permissions and define access rights to the database objects, ensuring data security and integrity. 


What is the difference between a Primary Key and a Foreign Key?

Primary Key
    A primary key is a column (or a set of columns) in a database table that uniquely identifies each record in that table. 
    
Foreign Key
    A foreign key is a column (or a set of columns) in one table that refers to the primary key in another table 


  What is an Entity-Relationship Diagram?
  An Entity-Relationship Diagram (ERD) is a visual representation of the structure of a database. It illustrates how entities (tables or objects) in a database relate to one another. ERDs are commonly used in database design to map out relationships between data and provide a clear model for developers, analysts, and stakeholders to understand the data architecture.


  

What are the advantages of relational databases?

Data Integrity

     Relational databases use constraints (like primary keys, foreign keys, and unique constraints) to ensure data integrity. These constraints enforce rules that help maintain accurate, consistent, and reliable data. For example, a primary key ensures that each record is unique, while a foreign key ensures that relationships between tables remain consistent.

2. Structured Query Language (SQL)

     Relational databases use SQL, a standardized language for managing and manipulating data. SQL provides a powerful and flexible way to query, insert, update, and delete data. It makes it easier for developers and analysts to interact with the database without worrying about the underlying implementation.

3. Flexibility and Scalability

     Relational databases are flexible in terms of schema design and data modeling. New tables, columns, or relationships can be added as needed without affecting the overall system. Many relational databases can also scale to handle large datasets, either through vertical scaling (upgrading server resources) or horizontal scaling (distributed databases).

4. Data Redundancy Control

     Relational databases help minimize data redundancy by organizing data into separate, normalized tables. This means that data is stored in a way that reduces duplication, ensuring that updates, deletions, and insertions only need to be done once. The use of relationships between tables helps ensure that related data can be retrieved efficiently without unnecessary duplication.

5. Security

    Relational databases offer robust security features, such as user authentication, authorization, and access control. Administrators can define roles and privileges for different users, restricting access to sensitive data and ensuring that only authorized users can perform certain operations on the database.

6. Ease of Use and Maintenance

    Relational databases are often easier to use and maintain due to their mature ecosystem, extensive documentation, and strong community support. Tools and frameworks available for relational databases provide intuitive interfaces for database administrators and developers to manage data, perform backups, and optimize performance.

7. Data Consistency

     Relational databases ensure data consistency by adhering to ACID (Atomicity, Consistency, Isolation, Durability) properties. These properties ensure that transactions are processed reliably, even in the case of system crashes, ensuring that the database remains in a consistent state.

8. Data Relationships and Joins

     Relational databases excel at handling complex relationships between data stored in multiple tables. Using joins, data from different tables can be combined efficiently based on logical relationships (e.g., one-to-many or many-to-many), allowing for sophisticated queries and analysis.

9. Backup and Recovery

    Relational databases provide built-in features for data backup and recovery. Automated backup mechanisms, along with point-in-time recovery options, help ensure data protection and minimize data loss in the event of a failure.

10. Transaction Management

    Relational databases support transactions, which are a sequence of operations that are executed as a single unit. The ACID properties of transactions ensure that either all changes in a transaction are committed or none of them are, thus maintaining consistency and reliability in the database.


   State four types of data type used to store data in tables? 
   Integer
    Used to store whole numbers (both positive and negative)
    
    VARCHAR (Variable Character)
        Used to store variable-length strings of text.

       DATE
     Used to store date values (year, month, day). It does not store time information, just the date. 

     DECIMAL (or NUMERIC)
Used to store numbers with a fixed number of decimal places, often used for financial data. It provides exact precision, unlike floating-point types.


What is the purpose of a database management system (DBMS)?
The purpose of a Database Management System (DBMS) is to efficiently store, manage, and retrieve data, ensuring that data is organized, accessible, and secure

Data Storage, Retrieval, and Management

    The primary purpose of a DBMS is to provide a structured way to store data, allowing for efficient retrieval and management. It organizes data into tables, indexes, and other structures that make it easy to access and update when needed.

Data Integrity and Consistency

    A DBMS ensures that the data stored in the database remains accurate, consistent, and reliable. This is done through constraints, such as primary keys, foreign keys, and check constraints, which enforce rules that prevent invalid or inconsistent data.

Data Security

    DBMSs implement security features to control access to sensitive data. This includes user authentication, role-based access control, and encryption, ensuring that only authorized users can access or modify specific parts of the database.

Concurrency Control

    A DBMS ensures that multiple users can access and modify the database simultaneously without causing conflicts or corruption. It uses techniques like locking, transactions, and isolation levels to manage concurrent access and maintain data consistency.

Backup and Recovery

    A DBMS provides tools and mechanisms for creating backups of the database and recovering data in case of failures or disasters. This ensures that critical data can be restored and business operations can continue with minimal interruption.

Data Independence

    A DBMS provides data abstraction, separating the data from the applications that use it. This means that changes to the database structure (like adding or removing columns) can often be made without affecting the application logic.

Efficient Query Processing

    DBMSs optimize data retrieval using query processing techniques, such as query optimization and indexing, to ensure that queries are executed as efficiently as possible, even with large amounts of data.

Support for Multiple Users

    A DBMS allows multiple users and applications to interact with the database at the same time, managing data access and ensuring that operations are completed without errors or conflicts.

Data Redundancy Reduction

    A DBMS reduces data redundancy by organizing the data into normalized tables. This helps avoid duplicate data, leading to more efficient use of storage space and simplifying data management.

Transaction Management

    DBMSs provide transaction management features, which ensure that operations are completed as atomic, consistent, isolated, and durable (ACID). This helps maintain the integrity of the database, even in case of system failures or crashes.

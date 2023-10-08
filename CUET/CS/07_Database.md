# Database
Database is an organized collection of related data that represent some real world entity and can be stored and accessed electronically.

## Advantage of Database Management System over File System:
- DBMS provides **data redundancy**(same piece of data exists in multiple places) and **data consistency**(Data consistency refers to the accuracy, reliability, and correctness of data in a system or database.) while in File system data are redundant and inconsistent.
- File system does not allow sharing of data or **data sharing** is too complex while in DBMS data sharing is very easy and efficient.
- **Data Concurrency**(more than one user is accessing the data at same time)- Anomalies occur when change made by one user is lost due to change made by another user. File system does not provide any procedure to stop anomalies while DBMS provides a locking system to stop anomalies.
- DBMS allows retrieving data by just writing a small query while a File system program has to be written for every **Data Searching.**
- DBMS provides **Data Integrity**(constraints to be applied to data before insertion) while File systems do not.
- DBMS has a **Recovery Manager** that retrieves data when the system crashes making it another advantage over File system.
- DBMS provides **Data Security** by providing shielding to its data while File system nots.
- DBMS also provides **Backup** functionality while File System nots.
- DBMS provides different **multi user Interfaces** like GUI, application program interface.
- It is easily **Maintainable** due to its centralized nature making another advantage over File system.
## Key Terms
- **Data Dependency** : Data dependency in a database management system (DBMS) refers to the relationship between data elements within a database. It determines how changes made to one data element affect other data elements in the same database.
- **Data Isolation** : Data isolation refers to the concept of maintaining the integrity and separation of data in a database system. It ensures that concurrent transactions or operations on the data do not interfere with each other, and each transaction is executed in an isolated manner.
- **Data Independence**: Characteristic of being able to modify the schema at one level of the database system without altering the schema at the next higher level
- **Data Consistency** : Data consistency refers to the ability to guarantee the integrity of the data in a database system.
- **Data Inconsistency** : a situation where various copies of the same data are conflicting
## Concepts
- **Domain** : A domain is a unique set of values that can be assigned to an attribute in a database. For example, a domain of strings can accept only string values.
- **Tuple** : In DBMS, a tuple is just a row representing some associated data for a certain entity
- **Relation** : Tables in database is refferd as realtion.
- **Candidate Key** : candidate key is a column or a set of columns in a table that can uniquely identify each record or row in that table. It is a concept used in the process of designing and creating a relational database.
- **Primary key** : A primary key is attribute of table that has task to uniquely identify the tuple of that table. **Syntax -** 
    - **At column level:** <column_name><datatype> Primary key;  
    - **At table level:** Primary key(<column_name1>[,column_name>]....);  
- **Alternate Kay** : an alternate key is a column or a set of columns that can uniquely identify a record in a table. It is different from the primary key in that it is an alternative option for identifying records, but it does not serve as the primary means of identification.
- **Foreign Key** : A foreign key is the one that is used to link two tables together via the primary key. It means the columns of one table points to the primary key attribute of the other table. **Synatax** - 
    - Foreign KEY (attr_name) REFERENCES base_table_name(base_table_attr_name) ON DELETE SET NULL
    - Foreign KEY (attr_name) REFERENCES base_table_name(base_table_attr_name) ON DELETE CASCADE
## Relational Algebra
visit ![Relational Algebra JavaTpoint](https://www.javatpoint.com/dbms-relational-algebra)
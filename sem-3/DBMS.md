DBMS - database management system (create, store, retrieve, update, and manage databases)

Data : processed or organized into meaningful information.  
Database : An organized collection of related data that can be easily accessed, managed, and updated.  
Information : raw-data  

◯ 1-tier architecture : (1 layer)  
&nbsp;&nbsp;&nbsp;&nbsp;It is an architecture where the user, application, and database are on the same system, and the user directly interacts with the database.
&nbsp;&nbsp;&nbsp;database <-> server

advantages: simple, low-cost, easy to use
dis_advantages: single user, low security, no central data base, difficult to share

#_2-tier architecture : (2 layer)  
The client directly communicates with the database & The server manages the database and processes queries.
    client <-> network <-> database

advantages: easy to accsess, low cost, easy deployment, simple
dis-advantage: limited scalability, security issues, difficult maintanence

#_3-tier architecture : (3 layer)
The client sends requests to the Application Server, which then communicates with the Database Server. It is more secure, easier to manage, and is used for large web applications.
    Client <-> Application Server <-> Database Server

advantages: enhanced scalability, data integrity, better security, better security
dis-advantages: more complex, difficult communication, slower response, higher cost

#_Database system: it is the process of planning how data will be stored before creating a database.

#_ER model: (Entity Relationship Model)
it is a database design model used to plan and represent the structure of a database before creating it. It shows entities, attributes, and relationships using a diagram.
    ▭ - entity (it is a person, place, object, or thing & it's anything about which we store data in a database)
    ◇ - relationship (Relationship shows the connection between two entities)
    ⬭ - attribute (Attribute is the information or property of an entity)

#_Relational model: it stores data in tables with rows and columns.    

key : it is used to uniquely identify each row in a table.
primary key : Every relation should have a primary key to uniquely identify each tuple(rows).
super key : Super Key is a key that uniquely identifies each row and may have extra attributes.
candidate key : A Candidate Key is the smallest possible Super Key.
alternate key : that are not selected as the Primary Key are called Alternate Keys.
composite key : it is a key made up of two or more attributes.
foriegn key : it is an attribute in one table that refers to the Primary Key of another table.

SQL : (Structured Query Language)
it is a language used to create, retrieve, update, and delete data in a relational database.

advantages : Easy to Learn – Simple and easy syntax.
             Fast – Retrieves data quickly.
             Standard Language – Works with most databases.
             Secure – Controls access to data.
             Handles Large Data – Can manage large amounts of data.

dis-advantages : Complex Queries – Large queries are difficult to write.
                 Costly – Some SQL databases are expensive.
                 Not Good for Unstructured Data – Best for structured data only.
                 Performance Issues – Can become slow with very large databases.
                 Needs SQL Knowledge – Users must learn SQL commands.             

| aspect       | sql                    | nosql                            |
| :------------: | :----------------------: | :--------------------------------: |
| data model   | tabels(rows&colums)    | documents                        |
| schema       | fixed                  | flexible                         |
| scaling      | vertical               | horizontal                       |
| relationship | joins                  | Embedded documents or references |
| best for     | highly structured data | Evolving or semi-structured data |

#_sql catagories : 
DDL(Data Definition Language) - it is used to define the database structure. (Creates/changes the structure)
    CREATE, ALTER, DROP, TRUNCATE, RENAME

DML(Data Manipulation Language) - it is used to add, change, delete, and retrieve data from a database. (Changes the data)
    INSERT, UPDATE, DELETE

DQL(Data Query Language) - it is used to retrieve or view data from a database. (Views/retrieves the data)
    SELECT

DCL(Data Control Language) - it is used to control access and permissions in a database. (Gives/takes permissions)
    GRANT, REVOKE

TCL(Transaction Control Language) -  is used to manage transactions in a database. (Saves/undoes changes)
    COMMIT, ROLLBACK, SAVEPOINT

#_Clause :-
A clause is a part of an SQL query that does a specific job, like selecting, filtering, grouping, or sorting data.
e.g. - select, from, where, group by, having, order by, limit,  as, distinct

#_sql like operator :-
it is used to search for a specific pattern in text in SQL.
It is commonly used with the WHERE clause.

e.g. - 
    starts with ('a%')
    ends with ('%a')
    contains ('%a%')
    exactly one character ('_vi') -> returns names exactly letters ending at vi (e.g. - rutvi)
    second character is a ('_a%')
    exactly 5 characters ('_____')

    summary :
    <img src="sumry.png" width="500">

#_sql string function :-
upper() - it converts text into uppercase letters
lower() - it converts text into lower letters
length() - it counts the number of characters in a string
substring() - function extracts a part of a string

    summary : 
    <img src="fun.png" width="500">

#_sql case statement :-
it is used to apply conditions in SQL, similar to IF...ELSE.
it is used to implement conditional logic in SQL
- The first matching condition is returned.
- ELSE is optional.
- case can be used with select, where, order by, group by, having

    summary :
    <img src="case.png" width="500">

#_what is join : 
it combines data from two or more tables using a common column.
We use it to combine related data from different tables and get the required information in one result.
→ JOIN helps us get the complete information we need when that information is stored in different tables.

                  SQL JOINS
                      │
    ┌─────────────────┼─────────────────┐
    │                 │                 │
INNER JOIN       LEFT JOIN        RIGHT JOIN
                      │
              FULL OUTER JOIN
                      │
                CROSS JOIN
                      │
                 SELF JOIN

1. Inner join :- It is used to retrieve only those records that have matching values in both tables.

2. Left join :- It returns all records from the left table and only the matching records from the right table. If no match exists, the right table's columns contain NULL.
    (a) full outer join - It returns all rows from both tables. Matching rows are combined, and non-matching rows from either table are also included, with NULL in the columns where data is missing.
    (b) cross join - It returns all possible combinations of rows from two tables, where every row from the first table is combined with every row from the second table.
    (c) self join - It is used to join a table with itself to find relationships between rows in the same table.

3. right join :- It returns all records from the right table and only the matching records from the left table. If no match exists, the left table's columns contain NULL.

◯ SQL set operations :-
1. union : It is used to combine the results of two or more SELECT queries and return only unique rows, removing duplicates automatically.
→ sorting is required, & it has slower perfomance
2. union all : It is used to combine the results of two or more SELECT queries and return all rows, including duplicates.
→ sorting is not required, perfomance id fater
→ why unino all is faster? - It is faster because it does not need to check for and remove duplicate rows.
3. intersect(Only common rows) : It is used to return only the rows that are common to the results of both SELECT queries.
4. expect(First query − Second query) : It is used to return only the rows that exist in the first SELECT query but do not exist in the second SELECT query.
5. multiple union - You can combine multiple queries.

◯ rules of set operations :-
1. Both queries must return the same number of columns.
2. Corresponding columns must have compatible data types.
3. Column names come from the first SELECT statement.
4. ORDER BY is written only once, at the end.

◯ what is sql subquery :-
It is a SQL query written inside another SQL query. The inner query provides a result that the outer query uses to retrieve or modify data.

▢ why we use subquery - to Retrieve data based on another query, Compare values dynamically, Filter records, Use with SELECT, INSERT, UPDATE, and DELETE, exists(Returns TRUE if the subquery returns at least one row)
| in                      | exists                    |
| :-----------------------: | :-------------------------: |
| compare values          | Checks row existence      |
| Good for small datasets | Better for large datasets |

▢ types of subqueries :-
1. single row subquery : Returns only one value
2. multiple row subquery : Returns multiple rows
3. Correlated Subquery : Depends on the outer query
4. Nested Subquery : A subquery inside another subquery

◯ View :- It is a virtual table created using a SELECT statement. It displays data from one or more existing tables without storing the actual data itself in the view.

▢ why we use view : 
1. Hide sensitive information
2. Simplify complex queries
3. Reuse frequently used queries
4. Provide data abstraction
5. Restrict user access to specific columns

▢ Types of views :
1. Simple View - Based on a single table, No aggregate functions, Usually updatable
2. Complex View - Based on multiple tables, Uses JOIN, GROUP BY, Aggregate Functions etc, Usually not updatable

▢ advantages of view :
1. Shows customized data to users
2. Provides data abstraction
3. Reusable SQL
4. Simplifies complex queries
5. Improves security

▢ disadvantages of view :
1. Table changes may affect the view
2. Depends on underlying tables
3. Some views cannot be updated
4. Can be slower for complex queries

VIEW

V → Virtual Table
I → Improves Security
E → Easy Query Reuse
W → Works Like a Table

◯ Normalization :- It means dividing a large table into smaller, related tables to avoid storing the same data repeatedly.

◯ Functional dependency :- It is a relationship between two attributes in a table where one attribute uniquely determines the value of another attribute.

▢ Types of functinoal dependency : 
1. trival - if the right-side attribute is already included on the left side, it is called a Trivial Functional Dependency.
2. non-trival - if the right-side attribute is not included on the left side, it is called a Non-Trivial Functional Dependency.

◯ Armstrong's Axioms :- It help us find new relationships between attributes using the relationships we already know.

▢ There are 3 rules : 
1. Reflexivity Rule - The Reflexivity Rule produces Trivial Functional Dependencies because the right-hand-side attributes are a subset of the left-hand-side attributes.
→ It states that if Y ⊆ X, then X → Y holds

2. Augmentation Rule - if a Functional Dependency is true, adding the same attribute(s) to both sides keeps it true.
→ It states that if X → Y, then XZ → YZ 

3. Transitivity Rule - if X determines Y, and Y determines Z, then X also determines Z.

▢ Secondary rules :-
1. union rule - if X determines both Y and Z separately, then X also determines Y and Z together. (X→Y, X→Z, X→YZ)
2. decomposition rule - if X determines Y and Z together, then X also determines Y and Z separately. (X→YZ, X→Y, X→Z)
3. pusedotransetivity rule - if X determines Y, and W together with Y determines Z, then W together with X also determines Z. (X→Y, WY→Z, WX→Z)

◯ Anomalies :- They are errors or difficulties that happen because of unnecessary data duplication in a database.

▢ Types of anomalies :
1. inseartion - we cannot add new information to a table because some other required information is missing.
2. update - when the same data appears multiple times, we must update every row. If we miss even one row, the data becomes inconsistent.
3. deletion - when we delete one piece of data, other important information may also be lost.

→ Redundancy means storing the same data repeatedly in a database.

Rmember :-
→ Normalization: The process of organizing database tables.
→ Normal Forms: The rules or stages followed during normalization.

◯ Normal Forms :- It tell us how to structure database tables correctly.

▢ There are 4 types of normal forms :
1. 1NF - every cell in a table must contain a single, atomic value, with no repeating groups.
2. 2NF - every non-prime attribute must depend on the entire candidate key, not just a part of it.
3. 3NF - A non-prime attribute should not depend on another non-prime attribute when that creates a transitive dependency on the key.
4. BCNF(Boyce-Codd Normal Form) - every functinoal dependency must be a superkey (stronger version of 3NF)
→ Rule: For every non-trivial functional dependency X→Y, X must be a superkey.

◯ Decomposition :- It means splitting one table into two or more tables to satisfy normalization rules.

◯ Denormalization :- It is the process of intentionally adding redundant data to a database to improve read performance.

◯ diffrence between normalization and denormalization :-
| feature                 | normalization             | denormalization |
| :-----------------------: | :-------------------------: | --- |
| redundancy              | low                       | high |
| storage                 | less                      | more |
| read speed              | may require joins         | usually |
| data consistency        | better consistency        | more updates |
| updates                 | easy                      | harder |
| data integrity          | high                      | lower if not managed |

◯ diffrence between prime attribute and non-prime attribute :-
| prime attribute         | non-prime attribte        |
| :-----------------------: | :-------------------------: |
| that is part of at least one candidate key | that is not part of any candidate key |

◯ ACID (atomicity, consistency, isolation, durability) :-  
1. atomicity - It is a property of a database transaction that means “All or Nothing
   → It ensures that either all operations in a transaction succeed, or none of them take effect.
2. consistency - A transaction takes the database from one valid state to another valid state without violating database rules
3. isolation - when multiple transactions run at the same time, each transaction should behave as though it is running independently, while the database maintains correct results
4. durability - once the database confirms that data is saved, it should remain saved even if the system crashes

◯ What is transiction :- A transaction means performing one task in a database, where all the required operations must succeed together, or none of them should take effect.

◯ transiction state :- They are the different stages a database transaction passes through, from starting its operations to completing successfully or failing.
e.g. - active, partially commited, committed, failed, abort

◯ Recovery mechanisum :- It is a technique used by a DBMS to restore the database to a correct state after a failure.
→ transiction may fail because of system crash, power failure, hardware failure, sowftware error, transictino error

▢ There are 2 important recovery techniques :
1. shadow copy schema - It is a database recovery technique that maintains two copies of the database: an old copy and a new copy.
(a) old copy - The original database
(b) new copy - The copy on which the transaction performs updates

▢ how shadow copy works : DBMS creates new copy of database → the original copy remians unchanged → All updates are performed on the new copy.

▢ What happens if transiction aborts?
Delete the new copy, keep the old copy, the original database remains vaild.

▢ What happens if the transaction commits(If the transaction completes successfully)?  
Write the new database pages to disk, Update db-pointer so it points to the new database, The new database becomes the current valid database, Delete the old database copy.

▢ How does Shadow Copy provide Atomicity? 
If the transaction fails before commit, the pointer still points to the old database
If the transaction commits, the pointer points to the new database

▢ How does Shadow Copy provide Durability?
Crash before pointer update: The pointer still refers to the old database, so the uncommitted changes are not visible.
Crash after pointer update: The new database was already written to disk, so its committed changes remain available.

▢ disadvantage of shadow copy :- The main disadvantage is that copying the entire database for a small transaction

▢ db-pointer : It is a pointer maintained on disk that points to the current valid copy of the database.

2. log-based recovery - It is a recovery technique in which the DBMS maintains a log containing records of database operations.
→ A log is stored in stable storage so that the DBMS can use it to recover after a failure.
→ it supports operations like UNDO, REDO

▢ Types of logged base recovery :-
1. Deferred Database Modification - The DBMS records changes in the log first and updates the actual database later.
2. Immediate Database Modification - The DBMS may change the actual database while the transaction is still executing.

◯ Indexing :- It is a technique used in DBMS to find records quickly without searching the entire table.

                    INDEXING
                       |
          +------------+------------+
          |                         |
    Primary Index             Secondary Index
          |
    +-----+-----+
    |           |
  Dense       Sparse

Multi-Level Index
        ↓
   Index on Index

1. primary index :- The records in the data file are arranged in order based on a particular attribute, and the index helps us find those records quickly.
   (a) dense - It is an index that contains an index entry for every search-key value in the data file, Requires more storage
   (b) sparse - instead of storing an index entry for every record, it stores only a few entries, usually one for each data block, Requires less storage 

2. secondary index :- It is used when the data file is not physically sorted according to the search key.
   
◯ Diffrence between primary and secondary index :-
| primary index                                | secondary index                          |
| :--------------------------------------------: | :----------------------------------------: |
| Data file is sorted by search key            | Data file is not sorted by search key    |
| Can be based on primary or non-key attribute | Can be based on key or non-key attribute |
| Usually Sparse                               | Usually Dense                            |
| Clustering                                   | Non-Clustering                           |

◯ Multi-Level Indexing :- It is a technique in which an index is created on another index to make searching faster.

▢ Advantages of indexing :-
1. faster data retrival
2. Usually faster database performance
3. Improves performance of search operations
4. Useful for SELECT, WHERE, and JOIN operations

▢ Limitations of indexing :-
1. extra storage
2. INSERT, UPDATE, DELETE become slower

◯ What is query processing :- It is the process of converting an SQL query into an executable form and executing it to produce the desired result.

◯ Query optimization :- It is the process of selecting the most efficient execution plan for an SQL query.
→ reduce execution time, and imporove overall perfomance

▢ There are 2 types to optimize the query : 1. selection, projection
1. selection : selection checks a condition and returns only the rows that match it.
2. projection : It is the operation of selecting specific columns from a table.

▢ Diffrence between selection and projection :-
| selection                                    | projection                               |
| :--------------------------------------------: | :----------------------------------------: |
| selects rows                                 | selects columns                          |
| uses WHERE                                   | uses SELECT                              |
| Example: marks > 80                          | Example: name, marks                     |

◯ What is join proccesing :- 
when the required information is stored in different tables, a JOIN combines that information.

▢ Join alorithems :-
1. nested loop join - It compares each row of the first table with every row of the second table to find matching rows.
2. hash join - It uses a hash table to find matching rows efficiently, mainly for equality joins.
3. sort-merge-join - It sorts both tables by the join key and then merges them to find matching rows.

◯ Cost estimation :- DBMS checks different ways to execute a query and estimates which way will use fewer resources.

◯ What is Explain :- It helps us understand how MySQL plans to find the required data, which indexes it may use, and how many rows it estimates

▢ Types of explain : 
1. const - Single Row Access
2. ref - Uses an Index
3. range - Range Search
4. all - Full Table Scan

◯ What is concurrency controll :- It ensures that when many users access or modify the same data simultaneously, their transactions do not interfere with each other incorrectly.
→ benifits - better resource utilization

▢ problems - 
1. lost update - One transaction overwrites another transaction's update.
2. dirty read - A transaction reads data written by another transaction before it commits.
3. non-repetabel read -  A transaction reads the same row twice and gets different values.
4. phantom read - The same query returns a different set or number of rows because another transaction inserted or deleted matching rows.

◯ What is clustering :- Instead of depending on only one database server, we use multiple servers to help handle requests, improve availability, or share the workload.

▢ Why we need :- more users, more requests, large workloads, high avalability

◯ Replication :- It means creating and maintaining copies of the same database data on multiple servers.
→ advantages - data redundancy, load balancing, high avalability, scalability
→ disadvantage - high cost, complexity, network dependency, difficult maintanance

▢ How it works : It works by connecting multiple servers, called nodes, so they work together to handle database requests.

◯ What is database scaling :-
It is the process of improving a database system so that it can handle more users, more data, and more requests without becoming too slow.

◯ Connection pooling :- It means maintaining a group of reusable database connections so that applications do not need to create a new connection for every request.

◯ CQRS((Command Query Responsibility Segregation)) :- It is a design pattern that separates read operations from write operations so that each can be handled independently.

◯ Diffrence between horizontal scaling and vertical scaling :-
| horizontal scaling                                                                            | vertical scaling                                                                                                |
| :---------------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------------------------------------: |
| More servers                                                                                  | Bigger server                                                                                                   |
| The process of adding more servers to distribute workload and increase the system's capacity. | The process of increasing the hardware resources of an existing server to improve its capacity and performance. |
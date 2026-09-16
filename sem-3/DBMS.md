DBMS - database management system (create, store, retrieve, update, and manage databases)

data : processed or organized into meaningful information.
database : An organized collection of related data that can be easily accessed, managed, and updated.
information : raw-data

#_1-tier architecture : (1 layer)
it is an architecture where the user, application, and database are on the same system, and the user directly interacts with the database.
    database <-> server

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

       aspect   |       sql         |               Nosql
    ------------+-------------------+--------------------------------
     data model |tables(rowscolumns)|             Documents
       Schema   |      Fixed        |             flexible
       Scaling  |     vertical      |            Horizontal
    Relationship|       joins       |Embedded documents or references
      Best for  |highly structured  |Evolving or semi-structured data
                |        data       |                    

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

continue to file 10



create : it is used to create a database
use database : it selects a database to work with
create table : it creates a new table inside the database
alter table : it is sed to modify an existing table.




When designing a relational database, you need to consider where repeating data can occur, as when expanding the database, it will result in unnecessary use of storage space.

The way to fix this is by using two separate tables, and creating a **relationship** linking them.

Relationships in relational databases come in three forms:
- one to one - one field matches to another
- one to many - one field matches to many others
- many to many - many fields match to many others

the link between a field and a table is a **primary key**

There are three methods, or ==normal forms==, used for arranging data in tables within a database

the flat file before normalisation is 0NF, meaning it isn't normalised, and is stored as a flat file


### First normal form

The **first normal form** (1NF) requires that a table follows five rules:
1. All field names are unique
2. all values in fields should be from the same domain - same data type
3. values in fields should be atomic - 1 value per box / record field intersection
4. no two records can be copies of each other
5. each table needs a primary key - one or more fields used to uniquely identify each record

### Second normal form

Building on the first normal form, the second normal form (2NF) only requires that any ==partial dependencies== are removed

When all partial dependencies are removed, each table serves its own purpose

If multiple fields are dependent on a single field, that single field can be used as a primary key to a different table, splitting the table into two separate tables

### Third normal form

Adding onto the first and second normal form, the third normal form (3NF) requires that all ==transitive dependencies== have been removed

This is done by removing all data dependent on fields that are not used as keys


There are further levels of normalisation, although beyond a certain point data normalisation is unnecessary

most normalisation beyond 1NF involves removing any dependencies, simplifying the table by splitting it into several constituent tables, thus reducing duplicate data
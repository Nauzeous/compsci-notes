Databases often need to support multiple simultaneous users, and the largest databases have million of records and thousands of people accessing it

Users can be different access rights to a database
- some users can only query the database and run reports
- others can add and modify records
- and a small amount of people can delete records

it is important that the database continues to work, while making many **data transactions**

it is important that the process of data transactions do not cause a database to stop working reliably, either by being **inconsistent** or **corrupted**

irrespective of the data transaction, the **Database Management System** ensures that the data stored in the database remains consistent

the consistency of the database is also referred to as ==data integrity==, and is important to keep the database functional

# referential integrity

a key technique in ensuring data integrity in relational databases is known as ==referential integrity==

referential integrity concerns **accuracy** and **consistency** of data within the relationship between tables

## For example: 
	if a record is deleted but is referenced by another table, you are left with a 
	relation to a record that does not exist, resulting in inconsistent data

a way to keep the referential integrity is to enforce a ==cascade delete==, deleting all records related to it(by a primary key)  when a single record is deleted. this means that you will remove all relations leading to nothing, as all relations linking to the deleted record are deleted along with it

although cascade deletes can assist with removing many records at once for the sake of maintaining referential integrity, it can be ==dangerous== to use, as many unintended deletions can occur in one-to-many relationships

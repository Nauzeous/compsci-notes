**transaction processing** is the act of processing information that is divided into individual operations called ==transactions==

Every transaction can **only succeed or fail as a unit**, and cannot be **partially complete** e.g. only half the data is sent

All relational databases have specific base functionality, described by the acronym ==CRUD==
- Create
- Read
- Update
- Delete
each of these have corresponding SQL statements
- insert
- select
- update
- delete
respectively

To ensure data integrity, transaction processing in a DBMS must conform to a set of rules which are referred to using the acronym ==ACID==
- Atomicity
- Consistency
- Isolation
- Durability
These four rules describe the properties required by all database transactions, in order to maintain data integrity

## Atomicity

Atomicity of a transaction requires that a change to the database is either complete or not done at all, so there is ==no partially performed transactions==

## Consistency

**All instances** of the database must be kept up to date, so ==desyncs cannot occur==

If a desync occurs, a user could make an online money payment without being received by the seller

## Isolation

Simultaneous interacting transactions cannot interrupt each other, so they are treated like sequential events

This is enforced in many DBMS by using ==record locking==

record locking involves placing records in a read only state while being accessed. Once the transaction is completed, the lock is removed


## Durability

When a change is made to a database, ==the transaction cannot be lost== through a system failure like a power cut

durability is upheld by writing transactions to **permanent non-volatile** secondary storage, rather than storing the changes in RAM which does not persist when the power is turned off

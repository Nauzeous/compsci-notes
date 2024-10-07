Hashing is what is performed by a ==hashing function==

hashing converts a string of characters into a fixed-length value or key that represents the original string

a hashing function is an algorithm that hashes data, some examples are:
- SHA
- MD5

a small change will change the hash value entirely

The reason that hashing is not the same as encryption is that multiple inputs can produce the same hashed output, meaning that the original value cannot be entirely determined by the hash value, but instead narrowed down

### Why use hashing

hashing is important for obscuring data to hack attacks
if someone manages to access your hashed data, they cannot determine what the original data was

For example, a password could be stored in a database as a hashed value, and when trying to log in, the hash value of the entered password is compared to the hash value of the stored password

Even though multiple inputs could result in the same hash value, it is unlikely enough to be considered secure


Hashing is also important for quick searching, insertion and deleting items in data structures

by using hashing, it is quicker as you do not need to search an entire data structure, but instead apply the hashing function to find the item

hash tables provide O(1) time complexity, meaning they always take the same time to search
Reading
## Intro to password hashing

Define the term “hashing”.
Hashing is a one way function that takes an input of any size and produces an output of a fixed size.

Explain to a non-technical friend what a hash function does to a password.
It shreds it up to be glued back togethre later.
## bcrypt overview

What does it mean to ‘salt’ a password?
To make password hashing more secure by adding a random string to the password before hashing it.

What piece of information would a hacker need to access in order to find the ‘salt’ string for your passwords?
The salt is stored in the database along with the hashed password.

jBCrypt (the paragraphs and code example at the top of the page)

How does the Blowfish block cipher handle the increased computation speed of new computers?
It uses a key that is 448 bits long.
What are the issue with the two most commong password hashes for Java (“Java password hash” and “Java password encryption”)?
They are not secure enough.












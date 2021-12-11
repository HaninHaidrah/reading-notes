# Implementation: Hash Tables
## What hash table => 
- In computing, a hash table is a data structure that implements an associative array abstract data type, a structure that can map keys to values. A hash table uses a hash function to compute an index, also called a hash code, into an array of buckets or slots, from which the desired value can be found.

![img](https://yourbasic.org/algorithms/hash-table.png)


## How to implement => 
- Hashing is implemented in two steps:

    1. An element is converted into an integer by using a hash function. This element can be used as an index to store the original element, which falls into the hash table.
    2. The element is stored in the hash table where it can be quickly retrieved using hashed key.

       > hash = hashfunc(key)
       > index = hash % array_size

**In this method, the hash is independent of the array size and it is then reduced to an index (a number between 0 and array_size − 1) by using the modulo operator (%).**

![img](https://he-s3.s3.amazonaws.com/media/uploads/7ea3425.jpg)
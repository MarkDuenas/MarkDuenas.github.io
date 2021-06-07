# Hash Table

## What is a Hash Table

A hash table (hash map) is a data structure that implements an associative array abstract data type, a structure that can map keys to values. A hash table uses a hash function to compute an index, also called a hash code, 
into an array of buckets or slots, from which the desired value can be found.

## Implementation of Hash Table

Hashing is implemented in two steps:

1. An element is converted into an integer by using a hash function. This element can be used as an index to store the original element, which falls into the hash table.
2. The element is stored in the hash table where it can be quickly retrieved using hashed key.

## Steps of hashing and Saving data to Hash Table

1. Create new Hash that takes in total number of buckets(storage places);
2. Call `add()` method to insert a new value into hash table.
3. The value gets hashed by the `hash()` method and will return an integer that corresponds to the bucket number that this value will live in.
4. The value then gets assigned a spot in the hash table based on the hashed value.
5. If there are any collisions, then the value gets push in the same spot but added to the next value of the node.

## Collisions

Collisions occur when pairs of elements are mapped to the same hash value. These should be avoided. One way to prevent any errors is implementing Linked Lists to hold each values.



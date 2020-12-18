# Hashtables

A hashtable is a data structre used to store information in key/value pairs with (ideally) very efficient lookup time.

Key terms:

- __*hash*__ - the output of an algorithm that converts some incomming value and converts it into another value, either for security or for another reason
- __*bucket*__ - each index of an hashtable, which can hold multiple key-value pairs if a collision happens
- __*collision*__` - when more than one key gets hashed into the same location of a hashtable

Lookups within a hashtable have a O(1) time complexity.

The way it works is that any given key is hashed in a predictable way. When given some input the hashing algorithm might scramble that input into some value, and that value might not be able to be unscrambled, but any given input can always be scrambled the exact same way. This means that given the same exact input as something that has already been hashed can be located in O(1) time.

A collision occurs when two different input get hashed into the same output. A perfect hashing algorithm will hash any input into a __unique__ output, while a worst-case hashing algorithm will hash any input into the __same__ output.

When a collision happens, the new value of the key/value pair would replace the old value unless you store key/value pairs in the the bucket. Then you can store multiple hashes in the same bucket. This means you have O(1) lookup time when you have buckets with only 1 hash, but if you have multiple key/value pairs in the same bucket, you might get O(1) to get to that particular bucket, but then O(n) to search through that bucket.

Buckets can be implemented using a linked list where each node has a key/value pair. It's critical to store both the key and also the value because multiple keys can get you to the same bucket.

Hash map can have any amount of buckets. A hashmap with little buckets can have many collisions, and pack more key/value pairs into those buckets, where a hashmap with many buckets will have lots of empty ones, thus taking more space. This is called the __*load factor*__.

[<-- Back](../README.md)

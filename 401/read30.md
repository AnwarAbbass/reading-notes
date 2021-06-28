# Hash Table
- A hash table is a data structure that is used to store keys/value pairs.

![](data:image/png;base64,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)

## using of hash table
- Hold unique values
- Dictionary
- Library

## Creating a Hash
- Hashtable traditionally is created from an array.
- After you've created your array, do some sort of logic to turn that "key" into a numeric number value.
- Each index of the array contain “buckets”, and each of these “buckets” holds one key/value pair combination.
- When there is no entry in a specific bucket, the buckets (each index of the array) all start null

## Collisions
- Collision occurs when more than one key hashes to the same index in an array.
- Collisions are solved by changing the initial state of the buckets.
- Instead of starting them all as null we can initialize a LinkedList in each one.
- Now if two keys resolve to the same index in the array then their key/value pairs can be stored as a node in a linked list.
- Since different keys can lead to the same bucket it’s important to store the entire key/value pair in the bucket, not just the value.

## To Store Values
- Hash maps to this to store values:
  - accept a key.
  - calculate the hash of the key.
  - use modulus to convert the hash into an array index.
  - store the key with the value by appending both to the end of a linked list.

## To Read Values
- Hash maps do this to read value:
  - accept a key
  - calculate the hash of the key
  - use modulus to convert the hash into an array index
  - use the array index to access the short LinkedList representing a bucket
  - search through the bucket looking for a node with a key/value pair that matches the key you were given
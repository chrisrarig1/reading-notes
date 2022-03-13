# Hashtables

## What are they?

- Hashtables are a data structure similar to dictionaries with key value pairs. Nodes are used and are contained in Buckets

## Important Terms

- *Hash*: A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose. In the case of a hashtable, it is used to determine the index of the array.
- *Buckets*: A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket. An index could potentially contain multiple key/value pairs if a collision occurs.
- *Collisions*: A collision is what happens when more than one key gets hashed to the same location of the hashtable.

## Functions

- *Hashing*: This turns the key into a integer which is then used as the index of the key/value
    - Using ASCII to convert letters into integers and adding those together
    - Multiply this number by a prime number
    - Use modulo to get the remainder of the result, when divided by the total size of the array.
    - Use number as index
- *Collisions*
    - This occurs when there is already a Node at the given index.
    - When this does happen we invoke Linked List logic and make the new node into the current.next
- *Add*
    - Send key to the *Hashing* method
    - Use the index and place the new *Node* at that index
- *Find*
    - Send key to the *Hashing* method
    - Uses index and returns the values for that index
- *Contains*
    - Accepts a key
    - Returns Boolean if that key exists

## Size

- *Bucket Sizes*: The more buckets there are the less likely a collision occurs. There is no limit to the number of buckets

# Useful Links

- [Hashtables](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-30/resources/Hashtables.html)
- [What is a HashTable Data Structure](https://www.youtube.com/watch?v=MfhjkfocRR0)
- [Basics of Hash Tables](https://www.hackerearth.com/practice/data-structures/hash-tables/basics-of-hash-tables/tutorial/)
[githup page](https://ahmadlotfyfalah1998.github.io/reading-notes/)
Hash - A hash is the result of some algorithm taking an incoming string and converting it into a value that could be used for either security or some other purpose.<br>
In the case of a hashtable, it is used to determine the index of the array.<br>
<br>
Buckets - A bucket is what is contained in each index of the array of the hashtable. Each index is a bucket.<br>
An index could potentially contain multiple key/value pairs if a collision occurs.<br>
<br>
Collisions - A collision is what happens when more than one key gets hashed to the same location of the hashtable.<br>
<br>
### What Are they
Hashtables are a data structure that utilize key value pairs. This means every Node or Bucket has both a key, and a value.<br>
<br>
### Example
["Greenwood:98103", "Downtown:98101", "Alki Beach:98116", "Bainbridge Island:98110", ...]<br>
<br>
# Structure
### Hashing
Basically, a hash code turns a key into an integer. It’s very important that hash codes are deterministic: their output is determined only by their input.<br>
Hash codes should never have randomness to them. The same key should always produce the same hash code.<br>
<br>
### Creating a Hash
A hashtable traditionally is created from an array. I always like the size 1024. this is important for index placement.<br>
After you have created your array of the appropriate size, do some sort of logic to turn that “key” into a numeric number value. <br>
#### Here is a simplistic hashing algorithm:
<br>
Add or multiply all the ASCII values together.<br>
Multiply it by a prime number such as 599.<br>
Use modulo to get the remainder of the result, when divided by the total size of the array.<br>
Insert into the array at that index.<br>

#### Hash maps do this to store values:

accept a key<br>
calculate the hash of the key<br>
use modulus to convert the hash into an array index<br>
store the key with the value by appending both to the end of a linked list<br>
#### Hash maps do this to read value:
<br>
accept a key<br>
calculate the hash of the key<br>
use modulus to convert the hash into an array index<br>
use the array index to access the short LinkedList representing a bucket<br>
search through the bucket looking for a node with a key/value pair that matches the key you were given<br>

## Methods
set()<br>
get()<br>
has()<br>
keys()<br>
hash()<br>

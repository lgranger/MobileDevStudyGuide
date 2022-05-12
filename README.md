# MobileDevStudyGuide

*This is a study guide for mobile devs working in React Native, Android, and iOS. It is a work in progress.*

## Al & Data

### Hash Tables

##### What
A Hash Table is a data structure that uses a hash algorithm to generate indexes each key/value pair. A hash algorithm takes an input of variable size (often a string) and returns as an output a value in a fixed range. This allows a limited range of indexes to be generated from an infinate range of keys. It also means that collisions - multiple keys having the same index - is possible. One of the ways to solve for this in a hash table is called secondary chaining which uses a secondary data stucture, such as a linked list, as the value at each index, and then store each key/value pair in the linked list at it's index. Lookup then involves generating the index, and then itterating through the linked list at that location until the correct key/value pair is found.

Hash tables are useful for getting quick lookup on large sets of unordered data. They are not suitable for data whose keys can't be hashed or that needs to be sorted.

Other considerations for when to use a hash table: the avaliable hash function is very collison-prone because it is poor or because it is ill-matched to the data you have, the data will grow/shrink frequenly (leading to frequent resizing) [^1]

#### Android
[Android Developers Documentation: Hashtable](https://developer.android.com/reference/java/util/Hashtable)

#### iOS
[Apple Developer Documentation: Hashable](https://developer.apple.com/documentation/swift/hashable)

###### References
[^1]: [StackOverflow: When to use hash tables?](https://stackoverflow.com/questions/36189665/when-to-use-hash-tables)

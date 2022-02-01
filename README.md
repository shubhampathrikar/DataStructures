# Data Structures

## Array
An Array is a collection of items. The items could be integers, strings, DVDs, games, books—anything really. The items are stored in neighboring (contiguous) memory locations. Because they're stored together, checking through the entire collection of items is straightforward.

**Basic Array Operations**

***Insertion:***
Inserting a new element into an Array can take many forms:

1. Inserting a new element at the end of the Array: At any point in time, we know the index of the last element of the Array, as we've kept track of it in our length variable. All we need to do for inserting an element at the end is to assign the new element to one index past the current last element.

2. Inserting a new element at the beginning of the Array: To insert an element at the start of an Array, we'll need to shift all other elements in the Array to the right by one index to create space for the new element. This is a very costly operation, since each of the existing elements has to be shifted one step to the right. The need to shift everything implies that this is not a constant time operation. In fact, the time taken for insertion at the beginning of an Array will be proportional to the length of the Array. In terms of time complexity analysis, this is a linear time complexity: O(N), where N is the length of the Array.

3. Inserting a new element at any given index inside the Array: Similarly, for inserting at any given index, we first need to shift all the elements from that index onwards one position to the right. Once the space is created for the new element, we proceed with the insertion. Again, this is also a costly operation since we could potentially have to shift almost all the other elements to the right before actually inserting the new element. 

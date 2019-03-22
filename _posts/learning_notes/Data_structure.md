# Data Structure

**Linked List**

*Why use linked lists?*

- A linked list saves memory.  

  It only allocates the memory required for values to be stored.

- Linked list nodes can live anywhere in memory. 

  When the references are updated, each linked list node can be flexibly move to different address.

*Disadvantage*:

Linear look up time. When looking for a value in a linked list, you have to start from the begining of chain, and check one element at a time.

Header node can also represent the linked list that starts from it.

**Doubly Linked Lists**

*Advantage over linked list:*

- Can be traversed in both forward and backward direction
- The delete operation is more efficient 

*Disadvantage:*

- Everynode require extra space for the previous pointer
- All operations require an extra pointer to be maintained




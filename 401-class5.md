# Linked Lists
- A linked list is a data structure that contains nodes (individual items/links) that links/points to the next node in the list.
- Linked lists are linear data structures.
- Linked lists don’t need to take up a single block of memory; instead, the memory that they use can be scattered throughout.
- There are two types of linked lists:
  - Singly - Each node has 1 reference, which points to the Next node in a linked list.
  - Doubly - Each node has 2 references to both the Next and Previous node.
- A node only knows about what data it contains, and who its neighbor is.
- Next - Each node contains a property called Next. This property contains the reference to the next node.
- Head - The Head is the first node in a linked list.
- A linked list is usually efficient when it comes to adding and removing most elements, but can be very slow to search and find a single element.

## Traversal
When traversing a linked list, you are not able to use a `foreach` or `for` loop. We depend on the Next value in each node to guide us where the next reference is pointing. The best way to approach a traversal is through the use of a `while()` loop. The `Current` will tell us where exactly in the linked list we are and will allow us to move/traverse forward until we hit the end.

![Linked Lists vs Arrays: from What’s a Linked List, Anyway? [Part 2]](https://miro.medium.com/max/1400/1*cUehR5S18XSoVLaPNfNzlA.jpeg)

Sources: [Linked Lists](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html) | [What’s a Linked List, Anyway? Part 1](https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d) | [What’s a Linked List, Anyway? Part 2](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996)
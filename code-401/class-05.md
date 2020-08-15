# Reading 5: Linked Lists

## Reading, Research, and Discussion

- **Linked List**: A sequence of _nodes_ that are connected (_linked_) to one another. Cricially, each node references the _next_ node in the link.

  - Two types of linked lists, each of which refers to the number of _references_ each node has:
    - **Singly**: Nodes only have one reference, and it points to the _next_ node in a linked list.
    - **Doubly**: Nodes have two references - which point to both the _next_ and the _previous_ node.

- **Node**: The individual items or links in a linked list. Contain data for each item or link. Each node contains at least a property called _next_, which references the next node in the list.

- **Properties of Nodes**:

  - **Next**: Each node has a property named **Next**
    - "Next" represents the next node
    - If "next" is ever **null**, it means that that node is the the last one in the list
  - **Head**: The **Head** is a property only of the _first_ node in a linked linked
  - **Current**: A reference to whatever node is being examined at this moment.

- **Traversing Linked Lists**

* _For loops_ cannot be used to traverse linked lists.
  - Instead, we use the "Next" value of nodes to "point" us to the next reference and guide the traversal of the list
* _While loops_ are the best method for travering linked lists
  - Continually check that the "next" node is not "null"

### Other Sources

- [Linked Lists](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html)

- [What's a Linked List, Anyway? (Part 1)](https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d)

- [What's a Linked List, Anyway? (Part 2](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996)

Return to the [Table of Contents](https://alex-whan.github.io/reading-notes/)

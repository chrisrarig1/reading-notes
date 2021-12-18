# Linked List Cheat Sheet

1. *Linked List*: data structure that contains nodes that links to the next node in the list
2. *Singly*: The number of references the node has. The node only has reference to the next node in the list
3. *Doubly*: The node has two references the next node and the node before
4. *Node*: Individual items that live in the list. Contains the data
5. *Next*: Reference to the next node
6. *Head*: Reference to the first node in the list
7. *Current*: Reference to the node that is currently being looked at

## Traversal:

- *Use*: While loops
- *Do not use*: For Each or For loops
- Code:`current <- Head`
`While Current is not Null`
    `If Include statement`
        `return TRUE`
    `Current <- Current.Next`
`Return FALSE`
- *Big O*:
  - **For Time**: Using Includes would be O(n). the n represents the number of nodes in the list
  - **For Space**: O(1) no additional space needed

## Adding a Node:

- *Use*: Add()
- Code:`newNode <- NEW Node`
`newNode.Value <- newValue`
    `newNode.Next <- Head`
    `Head <- newNode`

- *Use*: AddAfter() and AddBefore()
- Code: `AddBefore(newValue, valueToAddBefore)`
`Current <- Head`
`IF Current is equal to NULL`
    `return FALSE`
`WHILE Current.Next is not equal to NULL`
  `IF Current.Next.Value is equal to valueToAddBefore`
    `newNode <- NEW Node`
    `newNode.Value <- newValue`
    `newNode.Next <- Current.Next`
    `Current.Next <- newNode`
    `return TRUE`
  `Current <- Current.Next`
`return FALSE`

## Print Out Nodes

- *Use*: While loop
- Code:
`Print()`
`Current <- Head`
`While Current is not equal to NULL`
  `OUTPUT <- "{Current.Value}-->"`
  `Current <- Current.Next`
`OUTPUT <- "NULL"`

# Useful Links

- [Linked Lists](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/singly_linked_list.html)
- [Big O](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-05/resources/big_oh.html)
- [What Is a Linked List pt1](https://medium.com/basecs/whats-a-linked-list-anyway-part-1-d8b7e6508b9d)
- [What Is a Linked List pt2](https://medium.com/basecs/whats-a-linked-list-anyway-part-2-131d96f71996)
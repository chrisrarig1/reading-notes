# Trees Cheat Sheet

## Terms

1. **Node**: Contains its own value and a ref to the other nodes
2. **Root**: The node at the beginning of the tree
3. **K**: Max number of children any node may have i.e. Binary has k=2
4. **Left**: Ref to one child node in a binary tree
5. **Right**: ref to the other child node in a binary tree
6. **Edge**: the link between a parent and a child node
7. **Leaf**: node with no children
8. **Height**: the number of edges from the root to the furthest leaf

[Binary Tree](BinaryTree1.png)

## Traversals

- **Depth First**: Uses a stack to temporarily store nodes
    1. *Pre-Order*: `root>>left>>right`
    2. *In-order*: `left>>root>>right`
    3. *Post-order*: `left>>right>>root`
- **Breadth First**: Uses Queue to store nodes
  - Basically you are enqueue and dequeue until the Queue is empty
  - Code:
        `Queue breadth <-- new Queue()`
        `breadth.enqueue(root)`
        `while ! breadth.is_empty()`
            `node front = breadth.dequeue()`
        `OUTPUT <-- front.value`
        `if front.left is not NULL`
            `breadth.enqueue(front.left)`
        `if front.right is not NULL`
            `breadth.enqueue(front.right)`

## Binary Trees vs K-ary Trees

- Binary trees restrict the number of children to 2. K trees allow for more
- K Trees have a list of children rather than a left and right child
- Similar to above this consists of enqueuing and dequeuing each node an its children

## Adding a Node

- Fill all child spots from the top down using the breadth traversal and finding the first empty child and filling it
- For specific placement you need to reference the new node and the parent node

## Binary Search Trees

- All values larger than the root are placed to the right
- All values less than the root are placed to the left
- Searching the tree for a specific value entails comparing the node values while traversing through the tree. A while loop is the best method

# Useful Links

- [Trees](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)
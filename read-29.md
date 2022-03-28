# Graphs

- It is a non-linear data structure that can be looked at as a collection of vertices/nodes possibly connected by lin segments named edges

## Terms

1. *Vertex* - A vertex, also called a “node”, is a data object that can have zero or more adjacent vertices.
2. *Edge* - An edge is a connection between two nodes.
3. *Neighbor* - The neighbors of a node are its adjacent nodes, i.e., are connected via an edge.
4. *Degree* - The degree of a vertex is the number of edges connected to that vertex.

## Directed Graphs

- Graph where every edge is directed. Each node is directed to another node with a specific requirement

## Undirected Graphs

- A graph where the edges are connected but do not move in any direction

## Complete vs Connected vs Disconnected

- *Complete Graphs*: when all nodes are connected to all other nodes
- *Connected*: a graph that has all of vertices/nodes have at least one edge.
- *Disconnected*: a graph where some vertices may not have edges

## Acyclic vs Cyclic

- *Acyclic Graph*: A directed graph without cycles
  - **Cycle**:when a node can be traversed through and potentially end up back at itself
- *Cyclic Graphs*: A graph that has cycles
  - **Cycle**: defined as a path of a positive length that starts and ends at the same vertex

## Adjacency Matrix

- 2-dimensional array. n x n Boolean matrix
- Each Row and column represents each vertex of the data structure
- *Sparse*: graph is when there are very few connections
- *Dense*: graph is when there are many connections

## Adjacency List

- A collection of linked lists or array that lists all of the other vertices that are connected.

## Weighted Graphs

- A graph with numbers assigned to its edges
- Very similar to a key/value pair data structure

## Traversals

- *Breadth First*
  1. Enqueue the declared start node into the Queue
  2. Create a loop that will run while the node still has nodes present
  3. Dequeue the first node from the queue
  4. if the Dequeue‘d node has unvisited child nodes, add the unvisited children to visited set and insert them into the queue.
- *Depth First*
  1. Push the root node into the stack
  2. Start a while loop while the stack is not empty
  3. Peek at the top node in the stack
  4. If the top node has unvisited children, mark the top node as visited, and then Push any unvisited children back into the stack.
  5. If the top node does not have any unvisited children, Pop that node off the stack
  6. repeat until the stack is empty

# Useful Links

- [Graphs](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/graphs.html)
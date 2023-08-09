# Read Graphs:

## Introduction:
 A graph is a non-linear data structure consisting of vertices (or nodes) connected by edges. This structure allows for modeling various relationships between different elements.

### Terminology:

1. **Vertex (Node)**: A data object that can have zero or more adjacent vertices.
2. **Edge**: A connection between two nodes.
3. **Neighbor**: Nodes connected by an edge.
4. **Degree**: The number of edges connected to a vertex.

### Directed vs Undirected Graphs:

- **Undirected Graphs**: Edges are bi-directional, with no specific direction. Nodes are connected without a sense of order.
- **Directed Graphs (Digraphs)**: Edges are directed from one node to another. Arrows indicate the direction of the relationship.


### Types of Graphs:

- **Complete Graph**: All nodes are connected to every other node.
- **Connected Graph**: All nodes have at least one edge.
- **Disconnected Graph**: Some nodes may not have edges.

### Graph Representation:

- **Adjacency Matrix**: A 2D array representing the connections between vertices. 1 indicates a connection, 0 indicates no connection. Symmetric for undirected graphs.
- **Adjacency List**: A collection of linked lists or arrays listing connected vertices for each node.

### Graph Traversals:

**Breadth First Traversal:**

- Start at a specified vertex.
- Use a queue to traverse level by level.
- Mark nodes as visited to avoid cycles.
- Return the order in which nodes were visited.

**Depth First Traversal:**

- Start at a specified vertex.
- Use a stack to traverse deeper before backtracking.
- Mark nodes as visited to avoid revisiting.
- Return the order in which nodes were visited.
- Real World Uses of Graphs:

### Graphs have various practical applications:

1. **GPS and Mapping**: Finding routes, directions, and distances.
2. **Social Networks**: Representing connections between people.
3. **Airline Traffic**: Analyzing flight routes and connections.
4. **Recommendation Systems**: Suggesting products or content, as seen in Netflix.

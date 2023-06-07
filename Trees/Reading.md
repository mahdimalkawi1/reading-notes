# Read Trees:

## Introduction:
Trees are hierarchical data structures widely used in computer science. They consist of nodes connected by edges, forming a branching structure. In this discussion, we will cover the basics of trees, their traversal methods, and common types.

## What is a Tree?
A tree is a collection of nodes organized hierarchically. It has a root node and child nodes connected by edges.

## Tree Terminology:

- Node: Each element in the tree is called a node. Nodes can hold data and references to their child nodes.
- Edge: The connection between two nodes is called an edge. It represents the relationship between parent and child nodes.
- Root: The topmost node in the tree is called the root. It serves as the entry point for accessing the tree.
- Parent: A node that has one or more child nodes is called a parent node.
- Child: Nodes directly connected to a parent node are its child nodes.
- Leaf: A leaf node, also known as a terminal node, is a node with no children.
- Depth: The depth of a node represents the number of edges from the root to that particular node.
- Height: The height of a tree is the maximum depth among all the nodes in the tree.


## Tree Traversal Methods:

1- Depth-First Traversal:

- Pre-order: Current node, left subtree, right subtree.
- In-order: Left subtree, current node, right subtree.
- Post-order: Left subtree, right subtree, current node.

2- Breadth-First Traversal:

- Level-order: Visit nodes level by level.

## Common Types of Trees:

- Binary Tree: Each node has at most two child nodes.
- Binary Search Tree (BST): Left child contains smaller values, right child contains larger values.
- AVL Tree: Self-balancing binary search tree.
- Heap: Complete binary tree with heap property.
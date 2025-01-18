# Binary Search Tree (BST) Implementation

This project provides an implementation of a Binary Search Tree (BST) in C++ with various functionalities including insertion, searching, traversal, and range-based operations.

## Files Overview

### 1. `BST.hpp`

**Purpose**: Defines the structure of the BST and its operations.

**Key Features**:
- **Struct Node**: Represents a tree node with key, left, and right pointers.
- **Class BST**: Contains methods for BST operations and a private root node.

**Public Methods**:
- `BST()`: Default constructor.
- `BST(int data)`: Parameterized constructor to initialize a tree with a root node.
- `~BST()`: Destructor to free allocated memory.
- `addNode(int)`: Inserts a new node into the tree.
- `searchKey(int)`: Checks if a key exists in the tree.
- `printTree()`: Prints the tree in in-order traversal.
- `print2DUtil(int)`: Prints the tree in a 2D rotated format.
- `findKthSmallest(int k)`: Finds the k-th smallest element in the tree.
- `rangePrint(int k1, int k2)`: Prints all elements within a specified range.

### 2. `BST.cpp`

**Purpose**: Implements the methods declared in `BST.hpp`.

**Highlights**:
- **Helper functions for recursion**:
  - `addNodeHelper(Node*, int)`
  - `printTreeHelper(Node*)`
  - `searchKeyHelper(Node*, int)`
  - `kthSmallestHelper(Node*, int*, int)`
  - `destroyNode(Node*)`: Frees memory in post-order traversal.
  - `createNode(int)`: Creates a new node with a given key.
  - `print2DUtilHelper(Node*, int)`: Prints a tree rotated by 90 degrees.

### 3. `driver.cpp`

**Purpose**: Demonstrates the functionality of the BST implementation.

**Features**:
- Creates a BST and inserts nodes from a predefined array.
- Performs in-order traversal.
- Tests the `findKthSmallest` function for correctness.
- Demonstrates range-based printing.

## How to Use

### Compilation and Execution

To compile and run the program, use the following commands:

```bash
g++ BST.cpp driver.cpp -o bst
./bst

# CS 46B Lab 12: Family Tree

## Description

This lab creates a family tree using a tree data structure. Each person in the family tree is represented by a `TreeNode`. Every node can have one parent and multiple children.

The program reads the family tree from a text file, displays the tree, and finds the most recent common ancestor between two people.

## What I Learned

- How to create and use a tree data structure
- How to use recursion to search through a tree
- How to connect parent and child nodes
- How to read data from a text file
- How to find the most recent common ancestor of two nodes
- How to use exceptions to handle invalid input

## Program Structure

### `FamilyTree`

The `FamilyTree` class stores the root of the tree and contains the main methods for reading and searching the family tree.

### `TreeNode`

The `TreeNode` class represents one person in the family tree. Each node stores:

- The person's name
- A reference to the person's parent
- An `ArrayList` of the person's children

Important methods include:

- `addChild(TreeNode childNode)`  
  Adds a child to the current node and sets the child's parent.

- `getNodeWithName(String targetName)`  
  Recursively searches the tree for a person with the given name.

- `collectAncestorsToList()`  
  Follows the parent references and stores all ancestors in an `ArrayList`.

- `toString()`  
  Prints the family tree with indentation.

## Input File Format

Each line in the input file must follow this format:

```text
parent:child1,child2,child3

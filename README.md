# Binary Trees
A binary tree is a tree data structure in which each parent node can have at most two children. Each node of a binary tree consists of three items:

-data item,

-address of left child,

-address of right child.

## Types of Binary Tree
1. Full Binary Tree

    A full Binary tree is a special type of binary tree in which every parent node/internal node has either two or no children.

2. Perfect Binary Tree

    A perfect binary tree is a type of binary tree in which every internal node has exactly two child nodes and all the leaf nodes are at the same level.

3. Complete Binary Tree

    A complete binary tree is just like a full binary tree, but with two major differences

    Every level must be completely filled
All the leaf elements must lean towards the left.
The last leaf element might not have a right sibling i.e. a complete binary tree doesn't have to be a full binary tree.
4. Degenerate or Pathological Tree

   A degenerate or pathological tree is the tree having a single child either left or right.

5. Skewed Binary Tree

   A skewed binary tree is a pathological/degenerate tree in which the tree is either dominated by the left nodes or the right nodes. Thus, there are two types of skewed binary tree: left-skewed binary tree and right-skewed binary tree.

6. Balanced Binary Tree

    It is a type of binary tree in which the difference between the height of the left and the right subtree for each node is either 0 or 1.


## Binary Tree Representation

A node of a binary tree is represented by a structure containing a data part and two pointers to other structures of the same type.

```
struct node
{
 int data;
 struct node *left;
 struct node *right;
};
```

# Requirements
## General
* Allowed editors: vi, vim, emacs
* All your files will be compiled on Ubuntu 20.04 LTS using gcc, using the options -Wall -Werror -Wextra -pedantic -std=gnu89
* All your files should end with a new line
* A README.md file, at the root of the folder of the project, is mandatory
* Your code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl
* You are not allowed to use global variables
* No more than 5 functions per file
* You are allowed to use the standard library
* In the following examples, the main.c files are shown as examples. You can use them to test your functions, but you don’t have to push them to your repo (if you do we won’t take them into account). We will use our own main.c files at compilation. Our main.c files might be different from the one shown in the examples
* The prototypes of all your functions should be included in your header file called binary_trees.h
Don’t forget to push your header file
* All your header files should be include guarded

# More Info
## Data structures
Please use the following data structures and types for binary trees. Don’t forget to include them in your header file.
### Basic Binary Tree

```
/**
 * struct binary_tree_s - Binary tree node
 *
 * @n: Integer stored in the node
 * @parent: Pointer to the parent node
 * @left: Pointer to the left child node
 * @right: Pointer to the right child node
 */
struct binary_tree_s
{
    int n;
    struct binary_tree_s *parent;
    struct binary_tree_s *left;
    struct binary_tree_s *right;
};

typedef struct binary_tree_s binary_tree_t;
```

### Binary Search Tree

```
typedef struct binary_tree_s bst_t;
```
### AVL Tree

```
typedef struct binary_tree_s avl_t;
```
### Max Binary Heap

```
typedef struct binary_tree_s heap_t;
````

# Contributors
* Lucy Maina

* Samson Ajulor
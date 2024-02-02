﻿# 0x1D. C - Binary trees

## Learning Objectives

- What is a binary tree
- What is the difference between a binary tree and a Binary Search Tree
- What is the possible gain in terms of time complexity compared to linked lists
- What are the depth, the height, the size of a binary tree
- What are the different traversal methods to go through a binary tree
- What is a complete, a full, a perfect, a balanced binary tree

## Requirements

- Allowed editors: vi, vim, emacs
- All your files will be compiled on Ubuntu 14.04 LTS
- Your programs and functions will be compiled with gcc 4.8.4 using the flags -Wall -Werror -Wextra and -pedantic
- All your files should end with a new line
- A README.md file, at the root of the folder of the project, is mandatory
- Your code should use the Betty style. It will be checked using betty-style.pl and betty-doc.pl
- You are not allowed to use global variables
- No more than 5 functions per file
- You are allowed to use the standard library
- In the following examples, the main.c files are shown as examples. You can use them to test your functions, but you don’t have to push them to your repo (if you do we won’t take them into account). We will use our own main.c files at compilation. Our main.c files might be different from the one shown in the examples
- The prototypes of all your functions should be included in your header file called binary_trees.h
- Don’t forget to push your header file
- All your header files should be include guarded


## Data structures

Please use the following data structures and types for binary trees. Don’t forget to include them in your header file.

- Basic Binary Tree
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

- Binary Search Tree
```
typedef struct binary_tree_s bst_t;
```

- AVL Tree
```
typedef struct binary_tree_s avl_t;
```

- Max Binary Heap
```
typedef struct binary_tree_s heap_t;
```

- Note: For tasks 0 to 23 (included), you have to deal with simple binary trees. They are not BSTs, thus they don’t follow any kind of rule.

- Print function

To match the examples in the tasks, you are given this function

This function is used only for visualization purposes. You don’t have to push it to your repo. It may not be used during the correction

# Tasks

## Mandatory
- 0. New node - [0-binary_tree_node.c](0-binary_tree_node.c/)
- 1. Insert left - [1-binary_tree_insert_left.c](1-binary_tree_insert_left.c/)
- 2. Insert right - [2-binary_tree_insert_right.c](2-binary_tree_insert_right.c/)
- 3. Delete - [3-binary_tree_delete.c](3-binary_tree_delete.c/)
- 4. Is leaf - [4-binary_tree_is_leaf.c](4-binary_tree_is_leaf.c/)
- 5. Is root - [5-binary_tree_is_root.c](5-binary_tree_is_root.c/)
- 6. Pre-order traversal - [6-binary_tree_preorder.c](6-binary_tree_preorder.c/)
- 7. In-order traversal - [7-binary_tree_inorder.c](7-binary_tree_inorder.c/)
- 8. Post-order traversal - [8-binary_tree_postorder.c](8-binary_tree_postorder.c/)
- 9. Height - [9-binary_tree_height.c](9-binary_tree_height.c/)
- 10. Depth - [10-binary_tree_depth.c](10-binary_tree_depth.c/)
- 11. Size - [11-binary_tree_size.c](11-binary_tree_size.c/)
- 12. Leaves - [12-binary_tree_leaves.c](12-binary_tree_leaves.c/)
- 13. Nodes - [13-binary_tree_nodes.c](13-binary_tree_nodes.c/)
- 14. Balance factor - [14-binary_tree_balance.c](14-binary_tree_balance.c/)
- 15. Is full - [15-binary_tree_is_full.c](15-binary_tree_is_full.c/)
- 16. Is perfect - [16-binary_tree_is_perfect.c](16-binary_tree_is_perfect.c/)
- 17. Sibling - [17-binary_tree_sibling.c](17-binary_tree_sibling.c/)
- 18. Uncle - [18-binary_tree_uncle.c](18-binary_tree_uncle.c/)

## Advanced
- 19. Lowest common ancestor - [100-binary_trees_ancestor.c](100-binary_trees_ancestor.c/)
- 20. Level-order traversal - [101-binary_tree_levelorder.c](101-binary_tree_levelorder.c/)
- 21. Is complete - 102-binary_tree_is_complete.c
- 22. Rotate left - 103-binary_tree_rotate_left.c
- 23. Rotate right - 104-binary_tree_rotate_right.c
- 24. Is BST - 110-binary_tree_is_bst.c
- 25. BST - Insert - 111-bst_insert.c
- 26. BST - Array to BST - 112-array_to_bst.c
- 27. BST - Search - 113-bst_search.c
- 28. BST - Remove - 114-bst_remove.c
- 29. Big O #BST - 115-O
- 30. Is AVL - 120-binary_tree_is_avl.c
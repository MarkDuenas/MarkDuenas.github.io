# Binary Trees

## Terminology

- Node - A Tree node is a component which may contain it’s own values, and references to other nodes
- Root - The root is the node at the beginning of the tree
- K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
- Left - A reference to one child node, in a binary tree
- Right - A reference to the other child node, in a binary tree
- Edge - The edge in a tree is the link between a parent and child node
- Leaf - A leaf is a node that does not have any children
- Height - The height of a tree is the number of edges from the root to the furthest leaf

## Traversals

***Depth First***

Depth first traversals is when you priorotize going through depth(height) of the tree.

- Pre-order: root -> left -> right
- In-order: left -> root -> right
- Post-order: left -> right -> root

***Breadth First***

Interates through the tree by going through each level of the tree node by node across the tree(width).

## Binary Search Tree

Type of tree that has some rules in place. In a BST, nodes are organized from smallest to largest. Smallest values always goes to the left child and larger values goes to the right.

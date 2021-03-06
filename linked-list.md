# Linked List

A Linked List is a sequence of Nodes that are connected/linked to each other. Each Linked List's `Node` references the next `Node` in the link.

# Terminology

There are two types of Linked List:
  1. Singly - refers to the number of references the node has. Singlys means there is only one reference and points to the `Next` node in a linked list.
  2. Doubly - Node has two references, `Next` and `Prev`.
  3. Node - Nodes are individual obj/item that contain data.
  4. Next - Each node has a property of `Next` which points to the next Node in the list.
  5. Head - Head is the begining of the List and assigned the first node.

# Traversal

The best way to approach a traversal is through the use of a `while()` loop. This allows us to continually check the `Next` node in the list is not null.
If we reach a null node, it means we have reached the end of the Linked List.


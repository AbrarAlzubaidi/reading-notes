# trees DS: 
- Node - A Tree node which has a value
- Root - The root is the node at the beginning of the tree
- K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
- Left - A reference to one child node, in a binary tree
- Right - A reference to the other child node, in a binary tree
- Edge - The edge in a tree is the link between a parent and child node
- Leaf - A leaf is a node that does not have any children
- Height - The height of a tree is the number of edges from the root to the furthest leaf

![tree](https://i.ytimg.com/vi/qH6yxkw0u78/maxresdefault.jpg)

## Traversals: There are two categories of traversals
1. Depth First:

 **three methods for depth first traversal:**

1. Pre-order: root >> left >> right
2. In-order: left >> root >> right
3. Post-order: left >> right >> root

***The most common way to traverse through a tree is to use recursion.and stack***

2. Breadth First: by going through each level of the tree node-by-node.

***breadth first traversal uses a queue***

## Binary Tree: 
Binary Trees restrict the number of children to two 

## K-ary Trees: 
Nodes are able have more than 2 child nodes

- big O for insert into tree `O(n)`
- big O for searching `O(n)`

## Binary Search Trees: 
 In a BST, nodes are organized in a manner where all values that are smaller than the root are placed to the left, and all values that are larger than the root are placed to the right.

- time complexity: O(log(n))
- space //  : O(1)


***resources***

[trees-DS](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-15/resources/Trees.html)
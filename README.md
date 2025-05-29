# Leaf-Similar-Trees

# Given the roots of two binary trees, determine if they are "leaf-similar." Two trees are leaf-similar if their leaf value sequences (the order of leaves from left to right) are the same.

 # Approach 
To solve this problem, I used a depth-first search (DFS) approach to traverse each tree and collect the leaf nodes in order. Here's how it works:

#        Traversal:
For each tree, perform a DFS to visit every node.
When a leaf node (a node with no left or right children) is found, its value is added to a list.

#      Comparison:
After collecting the leaf sequences for both trees, compare the two lists.
If they are identical, the trees are leaf-similar.

#     Key Insights
DFS is Efficient: DFS ensures we visit nodes in a left-to-right order, which is crucial for maintaining the correct sequence of leaves.
Leaf Identification: A leaf node is identified when both its left and right children are None.


#     Space & Time Complexity:
Time: O(N + M), where N and M are the number of nodes in the two trees.
Space: O(N + M) to store the leaf sequences.

#      Why This Problem Matters
This problem is a great way to practice tree traversal techniques and understand how to manipulate and compare tree structures. It also highlights the importance of recursion in solving tree-based problems.

Example
Tree 1:

    3
   / \
  5   1
 / \ / \
6  2 9 8
Tree 2:

    3
   / \
  5   1
 / \ / \
6  7 4 2

Leaf Sequence for Tree 1: [6, 2, 9, 8]
Leaf Sequence for Tree 2: [6, 7, 4, 2]
Result: False (sequences don't match)

This example shows how the order of leaves matters—even if the trees look similar, their leaf sequences might differ.

Final Thoughts
This solution is clean, efficient, and leverages fundamental tree traversal concepts. It’s a great example of how breaking down a problem into smaller steps (collecting leaves, then comparing) leads to an elegant solution.

Happy coding! 🌿

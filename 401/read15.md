#  Trees
## Common Terminology
* Node - A Tree node is a component which may contain it’s own values, and references to other nodes
* Root - The root is the node at the beginning of the tree
* K - A number that specifies the maximum number of children any node may have in a k-ary tree. In a binary tree, k = 2.
* Left - A reference to one child node, in a binary tree
* Right - A reference to the other child node, in a binary tree
* Edge - The edge in a tree is the link between a parent and child node
* Leaf - A leaf is a node that does not have any children
* Height - The height of a tree is the number of edges from the root to the furthest leaf

![](https://miro.medium.com/max/3516/1*tUBYCHi32Zj0B2UCw0qmlA.png)


## Traversals

* Traversing a tree allows us to search for a node, print out the contents of a tree.
* There are two categories of traversals when it comes to trees:
   * Depth First.
   * Breadth First.

![img](https://qph.fs.quoracdn.net/main-qimg-770386a52678c9c44552eef3452fd540)



## Depth First

* Here are three methods for depth first traversal:
   * Pre-order: `root >> left >> right`
   * In-order: `left >> root >> right`
   * Post-order: `left >> right >> root`

![](https://images.slideplayer.com/24/6977355/slides/slide_3.jpg)



## Breadth First

* Breadth first traversal iterates through the tree by going through each level of the tree node-by-node. 

![](https://i1.wp.com/algorithms.tutorialhorizon.com/files/2015/05/Tree-Traversals-BFS-e1514854406978.png?resize=300%2C284)

## Binary Tree Vs K-ary Trees
* Trees can have any number of children per node, but Binary Trees restrict the number of children to two (hence our left and right children).

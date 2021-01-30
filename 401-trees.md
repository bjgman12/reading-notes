## Trees


- Node - A node is the individual item/data that makes up the data structure
- Root - The root is the first/top Node in the tree
Left Child - The node that is positioned to the left of a root or node
= Right Child - The node that is positioned to the right of a root or node
- Edge - The edge in a tree is the link between a parent and child node
- Leaf - A leaf is a node that does not contain any children
- Height - The height of a tree is determined by the number of edges from the root to the bottommost node

### Traversals 

> there are two ways of doing this

 - depth first
 - breadth first

### Depth

 #### pre-order
  ![Breadth Algo](preOrder.png)
  - top down first left right second prio


 #### in-order
 - left up right prio up down second
 ![Breadth Algo](inOrder.png)

 #### post-order
 - left right prio then up
  ![Breadth Algo](post.png)


 ### Breadth

 - use a Q to for this approach

 - queue the nodes in each row  once row has been seen pop values then move to next row

 ![Breadth Algo](breadthAlgo.png)
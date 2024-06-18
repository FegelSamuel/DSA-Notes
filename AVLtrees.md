# AVL Trees
* AVL Trees are self-balancing binary trees
* The worst case of an unbalanced tree is O(n), which we want to avoid (literally the same as a linear search)
* The height of a balanced binary tree is O(log(n))
```mermaid
   graph TD;
      A-->B;
      A-->C;
      B-->D;
      B-->E;
      C-->F;
      C-->G;
```
## Balanced Binary Tree Characteristic
* For each node, the height of the left and right subtrees can differ at most 1. This is an AVL Tree
```mermaid
   graph TD;
      A-->B;
      A-->C;
      B-->D;
      B-->E;
      E-->G;
      C-->F;
```
* This tree violates the AVL idea, the root being the problem
```mermaid
   graph TD;
      A-->B;
      A-->C;
      B-->D;
      B-->E;
      E-->G;
```


## Origin
* This idea was developed by Adelson-Velskii and Landis in 1962
## Insertion
This is the original AVL tree
```mermaid
   graph TD;
   5-->2;
   5-->8;
   2-->1;
   2-->4;
   4-->3;
   8-->7;
```
I want to insert 6, but it violates the AVL property
```mermaid
   graph TD;
   5-->2;
   5-->8;
   2-->1;
   2-->4;
   4-->3;
   8-->7;
   7-->6;
```
**NEEDS TO BE CONTINUED**













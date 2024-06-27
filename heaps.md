# Priority Queues
* Priority Queues are like normal queues with their **insert** methods, but the concept of deleteMin and deleteMax exists, in which they return and delete the minimum or maximum priority
## Basic Model
![The highest ASCII value has the most priority](https://github.com/FegelSamuel/DSA-Notes/assets/126997597/cd4229db-c71f-4416-8c72-7c561d2d623e)
# Heaps
* A Heap is a complete binary tree data structure that satisfies the heap property: for every node, the value of its children is less than or equal to its own value. Heaps are usually used to implement priority queues, where the smallest (or largest) element is always at the root of the tree.
* Heaps start on Index 1
![Heap](https://github.com/FegelSamuel/DSA-Notes/assets/126997597/e60722b3-a185-41b1-be63-9339c4442848)
## Insertion
* Keep in mind, we have to keep the integrity of the structure and every node has to have a subtree that's larger (or smaller) order (heap property)
* When a normal insertion violates the heap property, do upwards or downwards swaps until the property is ok



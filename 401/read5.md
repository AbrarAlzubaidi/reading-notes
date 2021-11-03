# linked-list:
linked-list is sequence of nodes (that represent each element in the list). linked by each other to make as a chain

There are two types of Linked List 
1. Singly: you can imagine it like chain and it moves from left to right **OR** from right to left by pointer called **next**
2. Doubly: you can imagine it as a circular chain moves from left to right **AND** from right to left by 2 pointers: **next and previous**

## what is head pointer:
head pointer is a pointer to point/refers the first node in the list

it looks like this:

![linkelist](https://media.geeksforgeeks.org/wp-content/cdn-uploads/gq/2013/03/Linkedlist.png)

## what is the specification: 
- you can loop through it by for/while/forEach/map loops and check if the Next pointer == Null then stop looping and that means you reach the last node
- time complexity: O(n)
- space complexity: O(1)

- you can create a new node by `Add()` then append the value and the pointers.

## Advantages of Linked List
1. Dynamic Data Structure
2. Insertion and deletion of nodes are really easier.
3. No Memory Wastage


## Disadvantages of Linked List
1. More memory is required to store elements in linked list as compared to array
2. Elements or nodes traversal is difficult in linked list.
3. In linked list reverse traversing is really difficult



------------------------------


# Analysis of Algorithm Efficiency

efficiency is evaluated based on 2 factors:

1. Running Time (also known as time efficiency / complexity)
The amount of time a function needs to complete.

2. Memory Space (also known as space efficiency / complexity)
The amount of memory resources a function uses to store data and instructions

## Four Sources of Memory Usage during function run-time:
1. The amount of space needed to hold the code for the algorithm.
2. The amount of space needed to hold the input data.
3. The amount of space needed for the output data.
4. The amount of space needed to hold working space during the calculation.


**Big O**: The worst case analysis of algorithm efficiency.
**Big omega**: The best case analysis of algorithm efficiency.
**Big theta**: The typical or random case used for analysis of algorithm efficiency.
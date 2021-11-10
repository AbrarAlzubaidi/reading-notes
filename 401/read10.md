# stack
stack techniqe is **last in first out (LIFO)**

## what is stack?
imagin you have a books and you want to put it inside a box. so the box is stack !! and if you want to remove a book from the box you will remove the last one you added to the box

![stack](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRH9t8kUYVnWdt_yJUEiLsKEGT1RvHr1CbxVA&usqp=CAU)

stack has some methods to deal with like **push and pop**
push: when you add to stack
pop: when you remove from it

also it has a pointer called  **top of stack (tos)**

tos will update by 2 ways: if you push to stack it will increase by 1, esle if you pop from it it will decrease by 1

## pushing 
Pushing a Node onto a stack will always be an O(1) operation


    ALOGORITHM push(value)
    // INPUT <-- value to add, wrapped in Node internally
    // OUTPUT <-- none
    node = new Node(value)
    node.next <-- Top
    top <-- Node

## Poping: 

Popping a Node off a stack is the action of removing a Node from the top Pop O(1)


    ALGORITHM pop()
    // INPUT <-- No input
    // OUTPUT <-- value of top Node in stack
    // EXCEPTION if stack is empty

    Node temp <-- top
    top <-- top.next
    temp.next <-- null
    return temp.value


## IsEmpty O(1): 


    ALGORITHM isEmpty()
    // INPUT <-- none
    // OUTPUT <-- boolean

    return top = NULL

    
--------------------------------



# Queue
Queue is a linear structure which follows a particular order in which the operations are performed.The order is **First In First Out (FIFO)**


queue has some methods to deal with like **Enqueue and Dequeue**
Enqueue: when you add to stack 
Dequeue: when you remove from it

queue has front pointer to point at its front

## What is a Queue? 
imagin you are standing in a queue the first one will be serviced is the first one at the queue 

![Queue](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTnuMdKyzHLHrZUpZejM67H88naqnd7bLySjozau1U_tnaCr9gyvM2jBNBumeSx-MDo3w0&usqp=CAU)
## Enqueue O(1)


    ALGORITHM enqueue(value)
    // INPUT <-- value to add to queue (will be wrapped in Node internally)
    // OUTPUT <-- none
    node = new Node(value)
    rear.next <-- node
    rear <-- node


## Dequeue O(1)


    ALGORITHM dequeue()
    // INPUT <-- none
    // OUTPUT <-- value of the removed Node
    // EXCEPTION if queue is empty

    Node temp <-- front
    front <-- front.next
    temp.next <-- null

    return temp.value


## IsEmpty O(1)


    ALGORITHM isEmpty()
    // INPUT <-- none
    // OUTPUT <-- boolean

    return front = NULL
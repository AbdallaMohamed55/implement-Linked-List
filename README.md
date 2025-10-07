# implement-Linked-List
To study and implement Linked List

#  Aim 

To study the concept of linked lists and implement operations such as creation, insertion, deletion, and traversal using C++.

# Theory 

A Linked List is a linear data structure in which elements are not stored at contiguous memory locations. Instead, each element (called a node) contains two parts:

  1.Data – stores the actual value or information.

  2.Pointer (Next) – stores the address of the next node in the list.

The first node is known as the head, and the last node points to NULL, indicating the end of the list

  ## Types of Linked Lists:

    1. Singly Linked List: Each node points to the next node only.

    2. Doubly Linked List: Each node has two pointers — one to the next and one to the previous node.

    3. Circular Linked List: The last node points back to the first node, forming a circular structure.

  ## Advantages:

   * Dynamic memory allocation (size can change at runtime)
   * insertion and deletion compared to arrays

  ## Disadvantages:

  * Extra memory for pointers

  * Sequential access (cannot access directly by index)

# Algorithms:

## ALGORITHM TO ADD MULTIPLE NODES AT THE END OF A LINKED LIST

START

Define a structure Node with:

data → to store integer value

next → pointer to the next node

Define a pointer head and set it to NULL (empty list).

Repeat the following steps for each new value to be inserted:

Create a new node using dynamic memory allocation.

Assign the value to newNode->data.

Set newNode->next = NULL.

If head == NULL, set head = newNode.

Otherwise:

Set temp = head.

Traverse the list until temp->next == NULL.

Set temp->next = newNode.

After all insertions, traverse the list from head to NULL and display the data of each node.

Free the allocated memory by deleting all nodes one by one.

STOP

## ALGORITHM TO ADD MULTIPLE NODES AT THE START OF A LINKED LIST

START

Define a structure Node with:

data → to store integer value

next → pointer to the next node.

Initialize the list with head = NULL.

For each new value to be inserted at the start:

Create a new node using dynamic memory allocation.

Assign the value to newNode->data.

Set newNode->next = head.

Update head = newNode (new node becomes the first node).

After all insertions, traverse the list starting from head until NULL, printing the data of each node.

Free the allocated memory by deleting each node one by one.

STOP


# Procedure

  i/ Start the C++ compiler and open a new file.

  ii/ Write the above program code.

  iii/ Compile the program to check for syntax errors.

  iv/ Run the program to view the output.

  v/ Observe the linked list before and after insertion/deletion operations.

# Conclusion 

The experiment successfully demonstrates how linked lists can be used to manage memory dynamically. Unlike arrays, linked lists allow efficient insertion and deletion of elements without shifting data. This concept is fundamental in building more advanced data structures such as stacks, queues, and graphs.


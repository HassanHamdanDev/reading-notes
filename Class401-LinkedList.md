# Implementation: Linked Lists

## Big O: Analysis of Algorithm Efficiency

- Big O: The worst case analysis of algorithm efficiency.
- Running Time: The amount of time required for an algorithm to complete.
- Memory Space: The amount of memory resources required for an algorithm to complete.
- Input Size: Represented by the variable n, the total size of values used as parameters in an algorithm.
- Big Omega: The best case analysis of algorithm efficiency.
- Big Theta: The typical or random case used for analysis of algorithm efficiency.


## Linked Lists

### A Linked List : *is a sequence of Nodes that are connected/linked to each other. The most defining feature of a Linked List is that each Node references the next Node in the link*

* Linear versus non-linear data structures

```

When we organize our data into hashes , we’re implementing a non-linear data structure. Trees and graphs are also non-linear data structures that we traverse in different ways, but we’ll talk more about them in more depth later in the year. It can be helpful to think of arrays and linked lists as being similar in the way that we sequence data.

```

* Memory allocation in static versus dynamic data structures

*The fundamental difference between arrays and linked lists is that arrays are static data structures, while linked lists are dynamic data structures. It doesn’t need a set amount of memory to be allocated in order to exist, and its size and shape can change, and the amount of memory it needs can change as well.*

* Parts of a linked list

*A linked list is made up of a series of nodes, which are the elements of the list. The starting point of the list is a reference to the first node, which is referred to as the head. The end of the list isn’t a node, but rather a node that points to null, or an empty value. A single node is also pretty simple.*

*A node only knows about what data it contains, and who its neighbor is. A single node doesn’t know how long the linked list is, and it may not necessarily even know where it starts, or where it ends. Because a single node has the «address» or a reference to the next node, they don’t need to live right next to one another, the way that the elements have to in an array. Instead, we can just rely on the fact that we can traverse our list by leaning on the pointer references to the next node, which means that our machines don’t need to block off a single chunk of memory in order to represent our list.*

* Lists for all shapes and sizes


```

Like most things in software, depending on the problem that we’re trying to solve, one type of linked lists might be a better tool for the job than another. Singly linked lists are the simplest type of linked list, based solely on the fact that they only go in one direction. This can be helpful if we wanted to be able to traverse our data structure not just in a single track or direction, but also backwards, too. For example, if we wanted to be able to hop between one node and the node previous without having to go back to the very beginning of the list, a doubly linked list would be a better data structure than a singly linked list.


```

* Basic Big O Notation Equations

An O function is linear, which means that as our input grows , the space and time that we need to run that algorithm grows linearly.

* Growing a linked list


```
We already know what linked lists are made of, and how their non-contiguous memory allocation makes them uniquely different from their seemingly more popular cousin, the array. Well, just like with an array, we can add elements and remove elements from a linked list. But unlike arrays, we don’t need to allocate memory in advance or copy and re-create our linked list, since we won’t «run out of space» the way we might with a pre-allocated array. We know that a linked list is made up a single node, and a node always contains some data and, most importantly, a pointer to the next node or null.

```



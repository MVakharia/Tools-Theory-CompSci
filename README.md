# Tools-Theory-CompSci

### A repository for code and documents written while studying computer science and learning to use coding tools.

## Algorithms

### Recursion

- What is a call stack?
- What is an execution context?
- What is the 'base case' in recursion?
- What is the 'recursive step' in recursion?
- What is Big O Notation?

Make the following text easier to understand:

'In a recursive function, the “counting variable” equivalent is the argument to the recursive call. If we’re counting down to 0, for example, our base case would be the function call that receives 0 as an argument. We might design a recursive step that takes the argument passed in, decrements it by one, and calls the function again with the decremented argument. In this way, we would be moving towards 0 as our base case.'

- What is the difference between a stack overflow and a stack underflow?
- What is a queue overflow and what is a queue underflow, and what is the difference between them?
- What is the 'recursive case'?
- Do some practice drills on recursion.

### Merge Sort

- Continually breaks down an array into pieces by splitting it in half to form 'runs', 
and splitting the halves in half to form more 'runs' and so on, 
until each run is a list containing a single element. 
All of the runs are then recombined into a sorted list. 
- When merging two single-element lists, they are compared for size. 
- Array.slice is used in Merge Sort.

### Quick Sort

1. Select a item that wil act as the 'pivot'. 
2. Every item greater in value than the 'pivot' moves to the right of the pivot. 
3. Every item less in value than the 'pivot' moves to the left of the pivot. 
4. Once all items have been sorted into two new lists, find a new 'pivot' in each list.
5. This will gradually subdivide lists over and over again until everything is in order.

- Write some programs that implement Quick Sort on data sets of interest to you,
for example, trading cards.

### Other sorting algorithms

- What is intro sort?
- What is heap sort?

#### What is O(log n) time?

- It means that as your input size grows, 
the number of steps taken by the algorithm grows *much more slowly.*

- If you're searching through a thousand names, it might take 10 steps to sort: log(base2) of 1000 is around 10 steps.
- If you're searching a million names, it might only take 20 steps to sort: log(base2) of 1,000,000 is around 20 steps, which is only double.
- You'll see this level of speed for yourself when you're flipping through an Oxford dictionary:
with every page you flip to, you're checking if the first letter of the search word has a greater or smaller index,
and flipping to a new page once you know. This is called a **binary search**. 

### Binary search

1. Find the middle index.
2. Check the middle index.
3. Check interatively. 

### What is a binary tree?

- The four properties of a node in a binary tree: data, depth, left, and right. 
- How do we insert a value into a binary tree?
- How do we retrieve a node by value from a binary tree?
- The two ways of traversing a binary tree: 
'breadth-first' and 'depth-first', and how they're defined. 

### Graphs in terms of networks

- A graph, in terms of a network, is a web of connections. 
- A graph consists of nodes, represented as circles, and edges, 
represented as lines that link the nodes together.
- A graph is a data structure. 

### Graph traversal

- The three methods of traversing a graph:
'breadth-first search' (BFS), 'depth-first search' (DFS), and Dijkstra's algorithm.
- Graph search algorithms
- Preorder, postorder, and reverse post-order
- Depth-first traversal
- Breadth-first traversal
- Dijkstra's algorithm

If you want to practice with Dijkstra's algorithm before coding it, 
use pen and paper to sketch out a graph, with nodes, edges, and edge lengths.
Then, follow along with the Computerphile videos. 

- What is a min-heap?
- What is the runtime of Dijkstra's algorithm?
- How do we code the algorithm?

### Nodes

- How do we implement a node in JavaScript?
- How to set the next node: allowing it to be updated so it can be traversed
and used in more complex data structures.
- Validating the next node: making sure that it is of the correct datatype.
- Getting the next node.
- What can nodes be used for in video games?
Ask this question to generate ideas to use for your own exercises and experiments.

### Linked Lists

- Common operations on a linked list include adding nodes, removing nodes, 
finding nodes, and traversing (travelling through) the linked list.
- A linked list is made up of nodes. Each node has a pointer, which could be null, 
or point to another node. 
- If you want to remove a node from the middle of a singly linked list, 
you must edit the pointer on the preceding node so that it points to what is now the next node.
- If you want to add a node to the end of a singly linked list, 
you must edit the preceding pointer.
- When you add a node to the start of a singly linked list, 
you must set the pointer to point to what used to be the start of the list.
- With doubly linked lists, there will be two pointers per node:
one pointing up the list, and one pointing down.
- The **head** node is the **first** node,
and the **tail** node is the **last** node.

Implement a linked list in JS. We want to start off with a list
(or nothing) and be able to perform all four common operations.

- We would need a 'node' class, and a way to add, remove, find, and traverse nodes.
- How do we locate the head node,
then add a node to the head node to create a new head node?
- How do we locate the tail node, 
then add a node to the tail node to create a new tail node?
- How do we remove the head node and set the next node to be the new head node?
- We need to print each change to the console so we can track the status of the linked list.
- `LinkedList` should be a class, with functions like `printList`,
`addToHead`, `addToTail`, `removeHead`, and `removeTail`.

### Doubly Linked Lists

- What three things do we have to do when *adding* to the **head** of a doubly linked list?
Which nodes must be updated?
- The same question, but for the **tail** of the list? Which nodes must be updated?
- How do we *remove* the **head** or the **tail** of a doubly linked list?
- How do we *remove* from the **middle** of a doubly linked list? Which nodes need to be updated?
- How do we find and *remove* a specific node by its data?
- How do we print the nodes in the list in order from head to tail?
- How do we implement a doubly linked list in JavaScript?

### Queues

- What is a queue, in terms of nodes?
- How do we implement a queue in JavaScript?
- Define the three methods of interacting with a queue: 
**enqueue**, **dequeue**, and **peek**.
- A queue can be implemented using a linked list as the underlying data structure.
- What is a *bounded queue*?
- What is *queue overflow*? How do we avoid it?
- What is *queue underflow* How do we avoid it?
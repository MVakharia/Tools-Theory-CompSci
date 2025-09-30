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

### The Queue

- What is a queue, in terms of nodes?
- How do we implement a queue in JavaScript, using a try-catch to check for overflow or underflow?
- Define the three methods of interacting with a queue: 
**enqueue**, **dequeue**, and **peek**.
- A queue can be implemented using a linked list as the underlying data structure.
- What is a *bounded queue*?
- What is *queue overflow*? How do we avoid it?
- What is *queue underflow* How do we avoid it?

### The Stack

- Can be implemented using a linked list as the underlying data structure.
Why is this better than an array or a list?
- The top of the stack is equivalent to the head node of the linked list.
- The bottom of the stack is equivalent to the tail node of the linked list.
- What causes a **stack overflow**?
- What causes a **stack underflow**?
- A stack has three main operations: push, pop, and peek. (what do these operations do?)
- How do we implement a stack in JavaScript, using a try-catch to check for overflow or underflow?

## Complex Data Structures

### Hash Maps

- What is a hash map?
- How can we use a hash map to efficiently store and retrieve data?
- The most efficient structure for storing and retrieving data. 
- It maps keys to their related values.

#### Maps

- If you have a table of cities with their respective countries,
each city can be mapped to a single country.
But it doesn't work the same way in the other direction:
one country can be mapped to multiple cities if those cities share a country. 
- Where the cities are the keys and the countries are the values,
each key can only be mapped to a single value.
One city cannot exist in two countries, but one country can contain two cities. 

This is what it takes for a relationship to be a map. 

- What kind of map is still a map when the keys and values are reversed?

#### Hash maps (continued)

- In the case of a map between two things,
we don't care about the exact sequence of the data: 
we only care that a given input, when fed into a map, produces the correct output.
- **You need to turn each key in your map into an index in your array.**


Imagine that you want the computer to remember that the card `Arcanite Magician` is `Super Rare`.

1. First, you take the card name and you turn it into a number. 
2. Let's say that the number we correspond with `Arcanite Magician` is `43`.
We find the 43rd index of the **array** we're using to store our map
and we save the property `Super Rare` there.
3. We get the number 43 by using a **hashing function**.
4. A hashing function turns a key into a number. 

For a hash map, the most important aspect is that
a hash function returns an array index as output. 

**Question**: Does the key to a hash table need to be a string?
Can you define a hash function that takes a different kind of input?

#### Hash functions

- Takes an input and returns a fixed-size value. 
- Can be a number, a string of characters, a binary buffer or byte array. 
- How do we write a hash function?

#### Hash maps (continued again)

- What are the main ingredients of a hash map?
  - Data that we want to preserve
  - A fixed-size array to insert the data into
  - A hash function.

#### Hash bucket

- A container used in a hash table to store entries that hash to the same index. 

#### Hash collisions

- When a hash function produces the same hash for two different keys.

#### Separate chaining

- Instead of storing a single value at each index, a linked list is stored.
- When there would be a collision between multiple keys with the same hash, 
the colliding key is placed in the same linked list as the one it collides with.

#### Saving keys

- Helps us check against the saved key when accessing data in a hash map. 
- Helps verify identity: when retrieving a value,
we hash the key and check the bucket. 
- If there are multiple entries,
we compare the saved key to the one we're searching for.
- Without saving the key, we wouldn't know which value belongs to which key.

#### Open addressing

- If there is a collision, we look for a new index to save the data
instead of saving multiple pieces of data in the linked list available at one index. 

##### Linear probing

- Continuing to find new array indices in a fix sequence until an empty index is found.

##### Other open addressing techniques

- Quadratic probing
- Double hashing
- Robin Hood hashing
- Cuckoo Hashing

What is clustering, in hash collisions?

How does a hash map turn the hash code for something into an array index?

#### Hash maps - programming exercises

- Create hashing functions in JavaScript that use the above techniques.
- Implement compression:
taking input and returning output only within a specific range.
- Create a method called `assign()`, which will assign a value to a generated index.
It must store the hashed key in a variable `arrayIndex`, and
assign the value to the element at `arrayIndex` in the hash map.
- Implement retrieval for your hash map
by defining and implementing a `retrieve()` function,
which will *retrieve* stored values.
- Implement a strategy to solve collisions
by updating the constructor and the `assign()` method.

##### Looping implementation

- Implement looping as a strategy to solve the problem of a
collision occurring when there are already values stored at a particular index. 
The values will be stored in nodes at these indices,
so we must loop over each node in the list to determine how to proceed.

The two possibilities we’ll encounter while looping are:

- The key we are looking for and the key of the current node are the same, so we should overwrite the value.
- No node in the linked list matches the key, so we should add the key-value pair to the list as the tail node.

After both cases, if we haven’t already exited the loop, we should reset the loop’s condition.

The `assign()` code for looping should look like this:
```
store the head node of the linked list in a variable, current 

while there is a current node
    if the current node's key is the same as the key
        store the key and value in the current
    if the current node is the tail node
        store the key-value pair in the node after the current

exit the loop      

set the current to the next node

```

##### Retrieval using `retrieve()`

- Different keys could point to the same array index,
leading to retrieval of the wrong value. 

`retrieve` method logic:

```
store the hashed key in the constant arrayIndex
store the head node of a list in the variable current

while there is a valid node
  if the current node's key matches the key
    return the current node's value
  set current to the next node in the list

return null
```



### Trees

- What is a tree?
- How can we use a tree to store hierarchical data?

### Min/Max Heaps

- What is a min/max heap?
- How do we implement a min/max heap?

### Graphs

- What is a graph?
- How do we represent complex data using a graph?
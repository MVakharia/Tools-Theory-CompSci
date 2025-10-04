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

'In a recursive function, the “counting variable” equivalent is the argument to the recursive call. 
If we’re counting down to 0, for example, our base case would be 
the function call that receives 0 as an argument. 
We might design a recursive step that takes the argument passed in, 
decrements it by one, and calls the function again with the decremented argument. 
In this way, we would be moving towards 0 as our base case.'

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
  - Stores hierarchical data with a directed flow. 
- How can we use a tree to store hierarchical data?
- What is a tree data structure?

What is a tree node?
- A very simple data structure that contains two things: **data**,
and a **list of children**, where each child is itself a tree node.


- What is an AVL tree?
- What is a red-black tree?
- What is a binary tree?
- **Directed flow** refers to the directionality of relationships between nodes:
the direction that the edges are flowing.
- In a tree structure, data moves **down**.
- In a tree, two nodes that share the same parent node are **siblings**. 
- In a tree, a node without children is referred to as a **leaf** node. 
- A **wide** tree has parent nodes referencing many child nodes.
- A **deep** tree has a lot of parent-child relationships, often single-child. 
- A tree can be both wide and deep. 
- Each movement from a parent to a child is a movement **down a level**. 
- Depending on the direction we're counting in,
we refer to this as either the **depth** or the **height**.
- We refer to it as the **depth** when we're counting levels down from the root node to the leaf node. 
- We refer to it as the **height** when we're counting levels up from a leaf node to the root node. 

#### Binary tree

- In a binary tree, a parent can have zero, one, or two children. 
- The two children are known as the left child and the right child. 
- In a **binary search tree**, a left child value must be **less than** its parent,
and a right child value must be **greater than** its parent. 
- At each node, we can discard **half** of the remaining possible values.
This makes the runtime O(log n).

#### Trees (continued)

- We can add data to a tree. 
- We can remove data from a tree.
- We can traverse the tree, depth-first.
- We can traverse the tree, breadth-first. 

Challenge: Create a `TreeNode` class in JavaScript.

- It must have **data**, **children**, 
a function that **adds children**, and a function that **removes children**. 

The generic steps to remove a child from a tree:

```

If target child is an instance of TreeNode,
  Compare target child with each child in the children array
  Update the children array if target child is found

Else 
  Compare target child with each child's data in the children array
  Update the children array if target child is found

If target child is not found in the children array
  Recursively call .removeChild() for each grandchild.

```

Because we implemented the children as an array, 
we can use the array `.filter()` method to update children. 
Like with `.addChild()`, we can also use `instanceof` 
to check if our target child is an instance of a `TreeNode`.

#### Pretty Print

Create a `print()` method that outputs the tree nodes like this:

```
15
-- 3
-- -- 6
-- -- 9
-- 12
-- -- 19
-- -- 8
-- 0
-- -- 10
-- -- 19
```

#### Depth-first tree traversal

Depth-first traversal visits the first child in the `children` array
and that node’s children recursively before visiting its siblings
and their children recursively.

The algorithm for depth-first traversal is as follows:

```
For each node
  Display its data
  For each child in the children array, call the method recursively
```

The above pretty-printed tree can be traversed depth-wise to produce this result:

```
15
3
6
9
12
19
8
0
10
19
```

**Challenge:** Implement a depth-first traversal function in your TreeNode class.

#### Breadth-first tree traversal

Breadth-first traversal visits each child in the `children` array
starting from the first child before visiting their children
and further layers until the bottom level is visited.
The algorithm is as follows:

```
Assign an array to contain the current root node
While the array is not empty
    Extract the first tree node from the array
    Display the tree node's data
    Append the tree node's children to the array
```

The tree from the previous exercise can be traversed breadth-wise to produce this result:

```
15
3
12
0
6
9
19
8
10
19
```

**Challenge:** Implement a breadth-first traversal function in your TreeNode class.

### Heaps

What is a heap?
- Used to maintain a minimum or maximum value in a dataset. 

Imagine you have a list of things to do, 
and you need to address these tasks in order of priority. 
A **priority queue** will ensure that you're always working on the most pressing assignment. 

Heaps are commonly used to create a priority queue.

Heaps tracking the maximum or minimum value are **max-heaps** or **min-heaps**. 

#### The max-heap

A heap that tracks the maximum value in a dataset is called a max-heap.

We can think of the max-heap as a binary tree with two qualities:

- The root is the maximum value of the dataset. 
- Every child's value is less than or equal to its parent.

#### The min-heap

A heap that tracks the minimum value in a dataset is called a min-heap.

We can think of the min-heap as a binary tree with two qualities:

- The root is the minimum value of the dataset. 
- Every child's value is greater than or equal to its parent. 

#### Adding elements to the heap

We can add up to two elements to a heap with only a root element.
The elements are added as children of the root element, from left to right.
The root makes up the first layer and the children make up the second layer.

Once the heap has three elements across two layers (the root and its two children),
we can add the third layer, which will be four elements going from left to right.
- Two of these elements will be the left and right children of the second layer's left element.
- The other two elements will be the left and right children of the second layer's right element.

#### Adding an element: Heapifying up

Sometimes we might add an invalid element to the heap: for example,
a child that is less than the value of its parent in a min-heap.

- In this case, the child value must move up the layers by swapping values with parent nodes
until the value is in the right place. In this case, it will be in the right place
once it is greater than or equal to its parent. This process is known as **heapifying**.

#### Removing an element: Heapifying down

The root node is the only element removed from a heap. 

Removing a root node is messy because both of its children become orphaned.
What we'll do instead is swap the root node's value with the value of the bottom rightmost element, which is the last element oin the array. 
Unfortunately, this might violate the rules of min-heaping if the newly swapped child's value is less than its parent.
If it does, we heapify down until the value is in the right place. 



#### Challenge: Implement a min-heap and a max-heap in JavaScript. 

Create a `MinHeap` class. It will store:
- An array of elements within the heap: `this.heap`
- A count of the elements within the heap: `this.size`

We'll always keep one element at the beginning of the array with the value `null`. 
- Why is this helpful?

`MinHeap` must satisfy two conditions:

- The element at index 1 is the minimum value in the entire list
- Every child element in the list must be larger than its parent. 

Define `MinHeap.add()`. It will add elements into the `MinHeap.heap` array.

Define `MinHeap.bubbleUp()`.
It will maintain the heap conditions as additional elements are added.

- `bubbleUp()` is called by `add()`, which appends an element to `.heap`. 
- `current` is defined within `bubbleUp()`. It points to the added element's index. 
- The initial value of `current` is the added element's current location (the end of `.heap`).

Define `MinHeap.popMin()`. It will pop the minimum value. 

Define `MinHeap.heapify()`. It will reform the heap if the root node is removed.

- The role of `heapify()` is similar to that of `bubbleUp()`. Look up the differences. 

When heapifying, we want to choose the correct child when faced with the
choice of either the left or right child.

- The correct choice is the smaller of the two children:
choosing the larger would stop us from maintaining our heap condition.

Define three helpers: `getParent()`, `getLeft()`, and `getRight()`:

```
const getParent = current => Math.floor((current / 2));
const getLeft = current => current * 2;
const getRight = current => current * 2 + 1;
```


### Graphs

A graph is a collection of nodes connected by edges. 

- How do we represent complex data using a graph?

Practice modeling a few more networks as graphs.

Imagine that you were asked to model a group of people as a social network, what would be the vertices and what would be the edges?

This is a tough one: how can you model a WiFi network?

In a **cycle**, a path begins and ends at the same vertex.
The vertex isn't connecting to itself with a single edge,
but across multiple vertices and edges that link back to the first vertex.

#### Weight

If the edges in a graph have a **value**, **number**, or **cost** associated with them, the graph is **weighted**.

- When tallying the total cost of a **path**, we add up the total cost of the edges used.
- In a weighted graph, the path with the least number of edges is not always the cheapest. 

#### Directed graphs

In a directed graph, the edges are always **one-way**. 

#### Representation of graphs

Graphs are typically represented in two ways: an **adjacency list** or an **adjacency matrix**.

##### Adjacency matrix

An adjacency matrix is a **table**.

- Each vertex in the graph is listed as both a row header
and a column header in the table. 
Therefore, the number of row and column headers are exactly the same. 
- A cell in the table is marked **true** or **false**
depending on whether the vertices listed in its corresponding row and column header
are connected.
- Since a vertex cannot connect to itself,
all cells where the row header matches the column header are marked as **false**. 
- If a cell's row and column header are vertices connected by an edge,
the cell is marked as **true**.
- In a weighted graph, the cells would be filled with numbers 
representing the edge weights. Where the edge is absent, the cell value is 0.

##### Adjacency list

- An adjacency list contains a list of the vertices as its keys. 
- In a graph without weight, paired to each key is an array of values
(where each value is a vertex)
- In a weighted graph, an array of objects is paired to each key,
where each object is a key value pair representing
each connected vertex and its distance from the key's vertex.

Challenge: Model graphs, both unweighted and weighted, in JavaScript. 

The graphs must have vertices, edges with costs in weighted graphs
and no cost in unweighted graphs.

Use an adjacency list to represent the graph.

Question: how would we model an adjacency matrix in JavaScript?
Is there any point when we can just use an adjancency list?

Create three classes: `Edge`, `Vertex`, and `Graph`.

The `Graph` class must be flexible enough to support **directed**, **undirected**, **weighted**, and **unweighted** graphs.
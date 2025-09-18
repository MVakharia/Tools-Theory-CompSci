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

- Write some programs that implement Quick Sort on data sets of interest to you, for example, trading cards.

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
4. 


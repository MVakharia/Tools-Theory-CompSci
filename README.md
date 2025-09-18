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

### Other algorithms

- What is intro sort?
- What is heap sort?


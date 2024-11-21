# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other?

its generaly faster to do DFS for sudoku. however if you have a lot of diffrent possible solutions without each thing having much to search after it might be better to do BFS. Another time could be finding something closest to the original input, meaning least moves, this would mean you want to start with the first moves and not want to go to deep.



2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?

its good to use data structures that bes fit the thing your doing because it can help make your code less confusing and make it faster. in this case we use a stack for DFS because we are going down one path for as long as possible. when we search one we find more possiblilites that we can explore. this is show with a stack because we immediatly add thoose possiblibilityes to the stack and look at them. when we run out of options that part of the stack is cleared and we go on to the next one. for BFS it helps to use a queue because you are looking at everything, one at a time, in the order that you find them.


3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?

you could expand it to anything that would have multiple possibilites. for example, the 9 sliding, where you would search possible moves, or even chess, where you could look at possible board possitions and evaluate what would be the best.
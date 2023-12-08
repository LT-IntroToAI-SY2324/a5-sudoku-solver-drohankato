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

Dfs might be preferred for use in a searching algorithm because of its characteristic deep search of a single brach, wheras Bfs might be preferred in a different type of search algorithm because of its exploration of all possibilities, level by level. Generally, i think the DFS searches performed more efficiently and found the answer using less moves than the BFS algorithm, but both varied heavily in tries per game. 


2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?

the stack is necessary for the Dfs algorithm because it allows it to follow a last in, first out procedure which helps it in trying to fill the most contrained cell with as many values as possible while also allowing it to backtrack through its mistakes. the queue allows Bfs to search through each possibility all on the same level at the same time. double ended queues could work for bfs also, which may allow it to search faster by searching on each end of the qeueue. 


3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges?

the board would definetely need to be adjusted and added to in order to have a more sophisticated grid based game, even an extension of the 9x9 sudoku board. These algorithms, which use data structures to find a solution to a constrained problem, could be used for real world applications involving logistics, scheduling, or any scenario which has a set of constraints .

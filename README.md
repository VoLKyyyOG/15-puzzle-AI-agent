# The IDA* Search Algorithm - Using it to Solve a 15-Puzzle (NP-Hard Problem)

For this project, I will be implenting an IDA* Search Algorithm to solve a 15-puzzle https://en.wikipedia.org/wiki/15_puzzle

These puzzles consist in assembling an image or some geometrical patterns, which has been decomposed
into a number of sliding tiles. We can consider each tile to be identified by a number, so we can
represent the initial state of the puzzle with the following diagram:  
![alt text](https://github.com/akiratwang/15-puzzle/blob/master/readme/init.PNG)

where B is a blank space. A puzzle solution is a sequence of moves which achieves the following state  
![alt text](https://github.com/akiratwang/15-puzzle/blob/master/readme/goal.PNG)  

subject to the constraint that we can only swap positions of the blank tile with some adjacent one.  

For instance, in the initial state depicted above, the only valid moves would be:  
1. Swap positions of tile 9 and blank B  
2. Swap positions of tile 14 and blank B  

Each possible configuration of the puzzle is called a state. The 15-puzzle Graph G = hV, Ei is implicitly
defined. The vertex set V is defined as all the possible puzzle configurations (states), and the edges
E connecting two vertexes are defined by the legal movements, also called actions or operators.  

The algorithm follows the Depth-First Search search strategy and is implemented as a recursive function (A control loop and a recursive function)  

The heuristic that I have used to prune the search space is the Sum of Manhattan Distances, as well as the Last Moves optimisation as suggested by the creator of the IDA algorithm (https://www.aaai.org/Papers/AAAI/1996/AAAI96-178.pdf)  

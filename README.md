# The IDA* Search Algorithm

For this project, I will be implenting an IDA* Search Algorithm to solve a 15-puzzle https://en.wikipedia.org/wiki/15_puzzle

The 15–puzzle
These puzzles consist in assembling an image or some geometrical patterns, which has been decomposed
into a number of sliding tiles. We can consider each tile to be identified by a number, so we can
represent the initial state of the puzzle with the following diagram:


where B is a blank space. A puzzle solution is a sequence of moves which achieves the following state




subject to the constraint that we can only swap positions of the blank tile with some adjacent one.
For instance, in the initial state depicted above, the only valid moves would be:

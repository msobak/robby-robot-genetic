# Robby the Can Cleaner

Robby the Can Cleaner is a robot living on a two-dimensional grid, where each cell is either empty, contains a can, or contains a wall. The edges of the grid are also considered to be walls. Robby's goal is to clean up the grid as well as possible, given the following constraints:
- Robby cannot move through walls.
- Robby only has vision of the cells that are adjacent to his current cells (not including diagonals).
- At each step, Robby can choose to either try move to one of his adjacent cells (not including diagonals), try to pick up a can in his current cell, or stay put and do nothing. He may attempt to move into a wall or pick up a can where there is none. He has no knowledge on how to do his job a priori, so even though such moves are obviously suboptimal, they are considered to be legal within the scope of the problem.

The code implements a genetic algorithm to train Robby to perform this task as well as possible. It was only optimized to the case where there are no walls inside the grid itself, though in principle it should work even if there are walls (although the random grid generator does not check whether the grid has areas that are completely enclosed by walls and thus unreachable for Robby). More details can be found in the PDF report.

The code is written in Wolfram Mathematica, as this was a requirement for the course.

This project was done together with Antonio Matosevic during our Bachelor's studies at Linneaus University in Sweden in 2015. 

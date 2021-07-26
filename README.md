# Solving-Puzzle-Games

## Purpose
The purpose of this assignment is for you to:
 Increase your proficiency in C programming, your dexterity with ecient memory allocation and
your algorithmic thinking, through programming a search algorithm over Graphs.
 Practice your ability to understand new algorithms based on those already taught in class.
 Gain experience with applications of graphs and graph algorithms to create an AI solver for a
game.
 Foster your capability to understand a scientic paper and implement its ideas (optional).

## Description
In this programming assignment you'll be expected to build a solver for the 15{puzzle https://en.
wikipedia.org/wiki/15_puzzle.
### The 15-puzzle
These puzzles consist in assembling an image or some geometrical patterns, which has been decomposed
into a number of sliding tiles. We can consider each tile to be identied by a number, so we can
represent the initial state of the puzzle and B is a blank space.
Each possible conguration of the puzzle is called a state. The 15-puzzle Graph G = (V,E) is implicitly
defined. The vertex set V is dened as all the possible puzzle congurations (states), and the edges
E connecting two vertexes are dened by the legal movements, also called actions or operators.

## Algorithm
Your solver should contain the implementation of the following search algorithm:
Iterative Deepening A* (IDA*)
The algorithm follows the Depth-First Search search strategy and can be easily implemented as a
recursive function.
IDA has two parts:
1. The main loop, initializes the thresholds B and B0 first. If no solution is found the search is
triggered again but with an updated B = B0 threshold.
2. The recursive function that implements the bounded Depth-First Search.
In this assignment IDA is guaranteed to nd the optimal solution. In general, IDA returns optimal
solutions as long as the heuristic function is a lower bound on the true optimal solution length (see
next section for more information on the heuristic used in this assignment).
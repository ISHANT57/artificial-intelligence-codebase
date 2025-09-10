A* Pathfinding Algorithm Implementation
This repository contains a Python implementation of the A* pathfinding algorithm applied to maze navigation problems. The implementation includes various heuristic functions to demonstrate how different heuristics affect the algorithm's performance and optimality.

Features
Standard A Algorithm* with Manhattan distance heuristic

Modified Heuristics:

Scaled Manhattan distance (1.5x multiplier)

Inconsistent Manhattan distance (violates consistency at specific nodes)

Visualization of paths found through the maze

Performance comparison between different heuristic approaches

Algorithm Details
A* Search Algorithm
A* is an informed search algorithm that finds the shortest path between two nodes in a graph. It uses a heuristic function to guide the search toward the goal more efficiently than uninformed algorithms.

Heuristic Functions
Manhattan Distance: The standard admissible and consistent heuristic for grid-based pathfinding

h(n) = |r₁ - r₂| + |c₁ - c₂|

Scaled Manhattan Distance: An inadmissible heuristic that multiplies Manhattan distance by 1.5

h(n) = 1.5 × (|r₁ - r₂| + |c₁ - c₂|)

Inconsistent Manhattan Distance: A heuristic that violates consistency at specific nodes

Adds an artificial penalty to nodes in the center region of the maze

Maze Representation
The maze is represented as a 2D NumPy array where:

0 = Passable path

1 = Impassable wall

Start position: (0, 0)

Goal position: (9, 9)

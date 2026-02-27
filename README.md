# Rat in a Maze – BFS (Queue)

This project was completed as part of my Data Structures & Algorithms term assignment (ITX 2010 / CSX 3003).  
The objective was to apply core data structure concepts — specifically **Queues** and **Breadth First Search (BFS)** — to solve a grid-based pathfinding problem.

## Problem

Given an `N x N` maze:

- `0` → open path  
- `1` → wall  

The rat starts at the top-left corner `(0,0)` and must determine whether it can reach the bottom-right corner `(N-1, N-1)` by moving up, down, left, or right.

The required output is strictly:

- `yes` if a path exists  
- `no` otherwise  

Constraints: `1 ≤ N ≤ 500` :contentReference[oaicite:0]{index=0}

## Approach

The maze is modeled as a graph using a 2D matrix.  
A queue-based BFS traversal is used to explore neighboring cells level by level.

Key components of the solution:

- Adjacency handling for four-directional movement
- Boundary validation to prevent out-of-range access
- Internal marking of wall cells
- Tracking visited cells to avoid reprocessing
- Termination logic based on whether the destination cell is explored

BFS was chosen because the maze is an unweighted grid, and BFS guarantees systematic exploration and shortest-path discovery.

## Results

Our final submission was evaluated on DMOJ:

- All test cases accepted  
- Maximum single-case runtime: **0.129s** :contentReference[oaicite:1]{index=1}

## Complexity

- **Time Complexity:** O(N²)  
- **Space Complexity:** O(N²)

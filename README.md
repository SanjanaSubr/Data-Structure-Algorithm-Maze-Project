# Data-Structure-Algorithm-Maze-Project
Assumption University - Sophmore Year DSA Course Project

Rat in a Maze – BFS (Queue) Implementation
Overview

This project solves the classic Rat in a Maze problem using Breadth First Search (BFS) with a Queue (FIFO) data structure.

Given an N x N maze:

0 represents an open path

1 represents a wall

The rat starts at the top-left corner (0,0) and must determine whether it can reach the bottom-right corner (N-1, N-1) by moving up, down, left, or right.

The program outputs:

yes

if a path exists, otherwise:

no
Problem Constraints

1 ≤ N ≤ 500

Grid size: N x N

Movement allowed in 4 directions (up, down, left, right)

Output must be strictly yes or no

This solution was evaluated on DMOJ and all test cases were accepted.
Maximum single-case runtime: 0.129s 

DSA Term project_ Rat in a Maze

Approach

The maze is treated as a graph where each cell is a node.

I implemented Breadth First Search (BFS) because:

The maze is an unweighted grid

BFS guarantees shortest-path exploration

It systematically explores all neighboring cells before moving deeper

A queue is used to:

Store valid positions

Process cells in FIFO order

Track step progression through the maze

Walls (1) are internally marked as -1, and valid moves are checked using boundary conditions to ensure coordinates remain inside the grid 

CodeLogicTermPRoject

.

If the bottom-right cell is explored, the program prints yes.
If the queue becomes empty before reaching it, the program prints no.

Time & Space Complexity

Time Complexity: O(N²)
Each cell is visited at most once.

Space Complexity: O(N²)
For the queue and visited tracking.

Example

Input:

4
0 0 1 1
0 0 0 1
0 1 0 0
1 0 0 0

Output:

yes
What This Project Demonstrates

Understanding of BFS vs DFS tradeoffs

Practical use of queues

Grid-based graph modeling

Boundary validation and state tracking

Competitive programming–style implementation

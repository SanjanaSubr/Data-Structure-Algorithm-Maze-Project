# Data-Structure-Algorithm-Maze-Project
Assumption University - Sophmore Year DSA Course Project

# Rat in a Maze – BFS (Queue)

Implementation of the classic **Rat in a Maze** problem using **Breadth First Search (BFS)**.

Given an `N x N` grid:
- `0` → open path  
- `1` → wall  

Starting at `(0,0)`, the algorithm determines whether the rat can reach `(N-1, N-1)` by moving up, down, left, or right.

The maze is modeled as a graph and solved using a queue-based BFS traversal.  
If the destination is reached → `yes`  
Otherwise → `no`

All test cases were accepted on DMOJ.  
Maximum runtime: **0.129s** :contentReference[oaicite:0]{index=0}

**Time Complexity:** O(N²)  
**Space Complexity:** O(N²)

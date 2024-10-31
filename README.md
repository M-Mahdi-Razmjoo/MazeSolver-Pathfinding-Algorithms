# MazeSolver-Pathfinding-Algorithms

## Project Description

MazeSolver is a Python project that implements various search algorithms—DFS, BFS, and A*—to solve a randomly generated maze. Inspired by the [Pacman](https://freepacman.org/) game, the goal is to help Pacman navigate from the start position (top-left) to the goal position (bottom-right). This project visualizes maze paths found by each algorithm and compares their performance based on expanded nodes, memory usage, and path costs.

## Features
- **Random Maze Generation**
- **Visualization of Search Paths**
- **Implemented Algorithms**: 
  - **Depth-First Search (DFS)** - Does not guarantee the shortest path
  - **Breadth-First Search (BFS)** - Guarantees the shortest path
  - **A* Search** - Uses heuristics to ensure the shortest and least costly path
- **Comparative Analysis**: Evaluates algorithms on expanded nodes, path length, and cost

## Project Structure

- **`MazeSolver.ipynb`**: Contains all code, explanations, and visualizations.
- **Classes**:
  - **`SearchAlgorithm`**: Base class that defines common methods for node exploration.
  - **`DFS`, `BFS`, `AStar`**: Classes inheriting from `SearchAlgorithm` to implement Depth-First Search, Breadth-First Search, and A* algorithms respectively.
  - **`SearchAlgorithmWithCosts`**: Base class for algorithms that account for cell-specific costs.
  - **`DFSWithCosts`, `BFSWithCosts`, `AStarWithCosts`**: Variants of the search algorithms that consider cell costs when calculating the optimal path.

---
## Algorithms Overview

### Depth-First Search (DFS)
DFS explores one complete path before backtracking, prioritizing depth over breadth. While DFS is memory-efficient, it does not guarantee the shortest path and can sometimes take longer to find a solution.

### Breadth-First Search (BFS)
BFS explores nodes level-by-level from the start, ensuring that the first time it reaches the goal is via the shortest path. However, it can be memory-intensive for large mazes due to the need to store all explored nodes.

### A* Search
A* uses a combination of path cost and heuristic estimates (such as Manhattan distance) to guide its search, making it one of the most efficient algorithms for finding the shortest and least costly path in a maze.


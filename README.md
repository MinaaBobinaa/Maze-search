## Overview

This Python script solves a maze problem using depth-first search (DFS). It reads a maze from a text file, finds the shortest path from the start ('A') to the goal ('B'), and outputs both a textual and image representation of the solution.

### Features:
- **Stack-based frontier (DFS)**: Explores each path until a dead-end is reached.
- **Queue-based frontier (optional for BFS)**: Can be easily switched by replacing `StackFrontier` with `QueueFrontier`.
- **Maze representation**: The maze is represented using ASCII characters.
- **Graphical output**: Outputs an image of the maze solution using the Python Imaging Library (PIL).

---

## File Structure

### Code Structure:
- **Node Class**: Represents a single state in the search tree.
- **StackFrontier Class**: Implements a stack for DFS search.
- **QueueFrontier Class**: Inherits from `StackFrontier` and overrides the `remove` method for BFS.
- **Maze Class**: Handles reading the maze, solving it, and outputting text-based and graphical solutions.

### Input:
The script expects a single argument, which is the filename of the maze to solve.

```bash
Usage: python maze.py maze.txt

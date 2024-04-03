# Maze Solver README

This project provides Python implementations of various maze generation and solving algorithms. It includes functionalities to generate mazes using depth-first recursive backtracking and binary tree algorithms. Additionally, it provides solvers based on uniform cost search and A\* search algorithms.

## Getting Started

To get started with this project, follow these steps:

1. **Clone the repository to your local machine:**
   https://github.com/jostbr/pymaze.
2. **Navigate to the project directory:**
   cd pymaze
3. **Install the required dependencies:**
   pip install -r requirements.txt

This project also requires `ffmpeg` for visualization. You can install `ffmpeg` using the following commands:

- **Linux**: `sudo apt install ffmpeg`
- **macOS**: `brew install ffmpeg`
- **Windows**: Download the [ffmpeg](https://ffmpeg.org/download.html) binaries and add them to your system PATH.

## Usage

You can use the provided algorithms to generate mazes and solve them.

### Generating a Maze

To generate a maze, you can use the `Maze` class with the desired algorithm. For example:

````python
from src.maze import Maze

maze = Maze(20, 20, algorithm="dfs_backtrack")
````

This will create a maze with dimensions 20x20 using the depth-first recursive backtracking algorithm.

### Solving a Maze

You can solve a generated maze using either uniform cost search or A* search algorithms. For example:

````python
from maze_solver import uniform_cost_search, a_star_search, manhattan_distance
````

# Solve using uniform cost search

### You can try applying different comments according to the algorithm you are using 
````python
solution_path, cost = uniform_cost_search(maze)
````
# Solve using A* search with Manhattan distance heuristic
````python
solution_path, cost = a_star_search(maze, manhattan_distance)
````



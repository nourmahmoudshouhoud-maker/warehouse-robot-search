# Warehouse Delivery Robot – Search Algorithms

Finds a path from S to G on a grid map using two search algorithms:

- **Uniform Cost Search (UCS)** – uninformed
- **A\*** with Manhattan-distance heuristic – informed

No path-finding libraries are used (only Python's built-in `heapq` and `time`).

## How to run

Open the notebook in Jupyter or Google Colab and click Run All.

Requires Python 3.8 or newer. No extra packages needed.

## How to change the map

Open `warehouse_robot.ipynb` and edit this line near the top:

    GRID = MAP_A      # change to MAP_B, MAP_C, or your own list of strings

Map symbols:

| Symbol | Meaning |
|---|---|
| `S` | Start |
| `G` | Goal |
| `.` | Normal floor (cost 1) |
| `~` | Rough floor (cost 3) |
| `#` | Wall (cannot enter) |

Section 7 of the notebook runs all three maps, and section 8 prints the results table.

## Output

For each algorithm the program prints:

- the algorithm name
- the path as a list of (row, column) from S to G
- path length and total cost
- the map with the path marked `*`
- nodes expanded, maximum frontier size, and run time

If no path exists it prints `No path found`.


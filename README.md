Robot Path Planning for Automated Part Sorting

This project simulates a basic warehouse-like robot tasked with collecting electronic components and delivering them to predefined drop-off zones. The robot navigates a grid while avoiding obstacles using the A* pathfinding algorithm.

 Overview

- A 20x20 grid environment is initialized.
- Random parts (`wire`, `switch`, `relay`) are placed in the upper-left section of the grid.
- Fixed drop-off zones are defined for each part type.
- A set of obstacles blocks the central area of the grid.
- The robot starts at position `(0, 0)` and:
  - Plans a path to each part using A*.
  - Picks it up and plans a path to the respective drop-off location.
  - Continues this process for all randomly placed parts.
- The paths are visualized using Matplotlib.

 Features

- Random part generation with part types and positions.
- A* pathfinding algorithm implementation.
- Obstacle avoidance.
- Grid-based visualization of parts, drop zones, obstacles, and paths.
- Outputs a data table with part type, pickup, and drop-off locations.

 📈 Visualization

The simulation includes:
- Blue circles representing part positions (labeled by type).
- Green squares for drop locations.
- Black squares as static obstacles.
- Colored paths representing the robot's movement.


## 📋 Dependencies

Install the required packages using pip:

```bash
pip install numpy matplotlib pandas

## 🧪 Running the Simulation
Run the simulation using:
python robot_sorting_simulation.py

## 🛠️ Possible Extensions
Add multiple robots with task allocation.

Implement dynamic obstacles or moving agents.

Use a GUI-based simulator for real-time control.

Replace A* with other algorithms like Dijkstra or RRT.



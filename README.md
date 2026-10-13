# Pathfinding & Maze Visualizer

An interactive maze game and pathfinding visualizer that runs entirely in a single `index.html`. It uses vanilla HTML, CSS and JavaScript, with no dependencies, build step or backend.

## Play

Open `index.html` in any web browser:

```bash
open index.html
```

1. Click **Start Game** to generate a random maze.
2. Move the blue player with the arrow keys or WASD, or click a neighbouring cell.
3. Reach the red goal to win. Match the shortest path for 3 stars.
4. Click **Show Optimal Path** to watch A* or Dijkstra solve the same maze.

## Explore mode

- Click and drag to draw or erase walls. Drag the green start and red end nodes to move them.
- **Generate Maze:** Recursive Division or Prim's algorithm.
- **Animate Search:** A* or Dijkstra, with an adjustable animation speed.
- After a search finishes, editing the grid updates the shortest path live.

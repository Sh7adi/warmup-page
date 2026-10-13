# MazeRunner

A maze game and pathfinding visualizer that runs entirely in a single file, `MazeRunner.html`. It uses vanilla HTML, CSS and JavaScript, with no dependencies, build step or backend.

## Play

Open `MazeRunner.html` in any web browser:

```bash
open MazeRunner.html
```

1. Choose a difficulty (**Easy**, **Medium** or **Hard**) and click **Start Game**.
2. Move the blue player with the arrow keys or WASD, or click a neighbouring cell.
3. Reach the red goal to clear the level. Clear all 5 levels to win.
4. Fewer moves earn more stars. Match the best possible route for 3 stars.
5. Click **Show Optimal Path** to watch A* or Dijkstra solve the same maze.

### Obstacles

- **Mud:** passable, but each step costs 3 moves. Sometimes a longer detour is cheaper.
- **Spikes:** lose a life and go back to the start. Running out of lives means game over.

Every level is guaranteed to be solvable. Spikes are only kept if a spike-free route to the goal still exists.

### Difficulty

| | Lives | Mazes | Spikes per level | Extra |
|---|---|---|---|---|
| Easy | 5 | Small | 0 → 4 | |
| Medium | 3 | Bigger | 2 → 10 | |
| Hard | 2 | Huge | 5 → 18 | Time limit |

Each of the 5 levels has a larger maze and more obstacles than the one before.

## Explore mode

- Click and drag to draw or erase walls. Drag the green start and red end nodes to move them.
- **Generate Maze:** Recursive Division or Prim's algorithm.
- **Animate Search:** A* or Dijkstra, with an adjustable animation speed.
- After a search finishes, editing the grid updates the shortest path live.

## Appearance

Use the **Light / Dark / Auto** switch in the header to choose a theme. **Auto** follows your system setting, and your choice is remembered for next time.

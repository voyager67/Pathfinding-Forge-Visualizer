# Pathfinding Forge

An interactive pathfinding and maze-visualization playground built with
HTML, CSS, and JavaScript.

**Goal:** make graph-search algorithms easier to understand by showing
how they explore a grid and discover a route from a start node to a
finish node.

## Features

-   Interactive grid for exploring paths and obstacles
-   Start and finish nodes
-   Wall placement and erasing
-   Random wall generation
-   Visualizations for Breadth-First Search (BFS), Depth-First Search
    (DFS), Dijkstra's algorithm, and A\* search
-   Playback controls: play, pause, step, reset, and animation speed
-   4-way and 8-way movement options
-   Search metrics and algorithm explanations

> This is an educational visualization tool. Results depend on the
> selected algorithm and movement settings. DFS does not guarantee a
> shortest path.

## Run locally

No build step or package installation is required.

1.  Download or clone this repository.
2.  Open `index.html` in a modern browser.
3.  Choose an algorithm and create a maze.
4.  Start the search using the app's pathfinding control.

If your browser restricts any feature when opening a local file, serve
the folder with a simple local HTTP server instead.

## How to use

1.  Set the start and finish positions.
2.  Draw walls or generate a random maze.
3.  Select a pathfinding algorithm.
4.  Choose 4-way or 8-way movement if available.
5.  Start the search and observe explored cells and the resulting route.
6.  Pause, step through the search, adjust speed, or reset to try
    another algorithm.

## Algorithms at a glance

  -----------------------------------------------------------------------
  Algorithm               General behavior        Shortest-path guarantee
  ----------------------- ----------------------- -----------------------
  BFS                     Explores in layers by   Yes, for unweighted
                          number of steps         grids with consistent
                                                  movement costs

  DFS                     Follows one branch      No
                          deeply before           
                          backtracking            

  Dijkstra                Expands the lowest      Yes, with non-negative
                          accumulated-cost node   edge costs

  A\*                     Uses accumulated cost   With a suitable
                          plus a heuristic        admissible/consistent
                          estimate                heuristic and matching
                                                  movement costs
  -----------------------------------------------------------------------

## Project structure

This is a static browser app. The main entry point is `index.html`,
alongside its CSS and JavaScript assets. Exact filenames may vary with
the repository layout.

## Testing checklist

-   Test a clear, unobstructed path.
-   Test a fully blocked or unreachable finish.
-   Try start and finish positions near grid edges.
-   Reset during and after a search.
-   Switch algorithms between runs.
-   Test both movement modes, if enabled.
-   Try small and large mazes.
-   Check narrow/mobile screens.

## Technology

-   HTML
-   CSS
-   Vanilla JavaScript
-   GitHub Pages for static hosting

## Roadmap

-   Expand automated tests for path correctness and unreachable
    destinations
-   Improve mobile and keyboard accessibility
-   Refine comparison metrics and step-by-step explanations
-   Add example mazes and usage documentation

## Contributing

Bug reports, suggestions, and pull requests are welcome. Please describe
the steps to reproduce a bug and include your browser/device details
when relevant. For algorithm changes, include a small test case that
demonstrates expected behavior.

## License

This project is distributed under the MIT License. See
[`LICENSE`](LICENSE) for details.

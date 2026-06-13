# Kruskal MST in C

Implementation of Kruskal's algorithm for finding the Minimum Spanning Tree (MST) of a weighted graph.

## About

This project demonstrates the implementation of Kruskal's algorithm in C. The algorithm constructs a Minimum Spanning Tree by repeatedly selecting the lowest-weight edge that does not create a cycle.

Kruskal's algorithm is a classic greedy algorithm widely used in graph theory, network design, and optimization problems.

## Features

* Graph edge processing
* Edge sorting by weight
* Cycle detection
* Minimum Spanning Tree construction
* Greedy optimization approach
* Console-based execution

## Algorithm Overview

Kruskal's algorithm works as follows:

1. Sort all graph edges by increasing weight.
2. Select the smallest edge.
3. Add the edge to the spanning tree if it does not create a cycle.
4. Repeat until the tree contains `V - 1` edges.

The resulting tree connects all vertices with the minimum possible total weight.

## Complexity

| Operation             | Complexity |
| --------------------- | ---------- |
| Edge Sorting          | O(E log E) |
| Union-Find Operations | O(E α(V))  |
| Total Complexity      | O(E log E) |

Where:

* `V` — number of vertices
* `E` — number of edges
* `α(V)` — inverse Ackermann function

## Project Structure

```text
.
├── main.c
├── README.md
└── project files
```

## Build

Using GCC:

```bash
gcc main.c -o kruskal
```

Run:

```bash
./kruskal
```

## Example

Input graph:

```text
A --1-- B
|       |
4       2
|       |
C --3-- D
```

Output:

```text
Minimum Spanning Tree:
A-B (1)
B-D (2)
C-D (3)

Total Weight: 6
```

## Applications

* Computer network design
* Road and railway planning
* Electrical network optimization
* Telecommunications
* Graph analysis

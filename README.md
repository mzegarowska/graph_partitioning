# Graph Partitioning & Analysis (Java)

A Java-based application dedicated to parsing, constructing, and partitioning graph structures using custom algorithmic logic. The project features robust file I/O engines for text and binary data, an adjacency matrix builder, and a custom graph partitioning algorithm driven by Dijkstra's shortest path calculations.

## Tech Stack & Concepts
- **Language:** Java (SE standard)
- **Core Concepts:** Object-Oriented Design (OOP), Custom Data Structures (Nested Node classes), Custom File I/O (Textual Buffered Readers & Binary Input Streams), Graph Theory.
- **Algorithms:** Dijkstra's Shortest Path Algorithm, Greedy/Distance-based Graph Partitioning.

## Team & Collaboration (Academic Project)
This project was developed in a two-person team for a Computer Science course focusing on algorithms and data structures.
- **My Contributions:**
  - Designed the core `Graph` data structures, including the static `Node` model with state-management for pathfinding metrics.
  - Developed the automated Adjacency Matrix builder (`generateAdjMtx`) and graph visualization components.
- **Teammate's Contributions:**
  - Implemented the custom graph definition parsers capable of reading structural grids and edge lists from plain text (`readtxt`) and byte-encoded files (`readbin`).
  - Implemented the custom graph partitioning algorithm (`partition_graph`) utilizing Dijkstra distance matrices to segment graphs into $k$ balanced sub-graphs.

## Features
- **Dual-Format Parser:** Dynamically processes graph structures from standard text logs (`.txt`) and raw byte streams (`.bin`) mapping matrix boundaries seamlessly.
- **Stateful Dijkstra Pathfinding:** Computes shortest paths from a source node, storing localized multi-partition distance matrices directly inside optimized node configurations.
- **Heuristic Graph Partitioning:** Evenly splits a broad graph into a user-defined number of sub-graphs ($k$) while obeying architectural constraints and distance-based grouping.
- **Adjacency Matrix Generator:** Generates mathematical bidirectional matrix tables directly from dynamic edge collections.

## Project Structure
- `Graph.java` - The main executable module containing the `Node` schemas, I/O engines, graph algorithms, and the `main` simulation setup.
- `res.txt` / `res.bin` - Dataset packages representing sample graph topographies used for system evaluation.

## How to Run Locally

### Prerequisites
Make sure you have Java Development Kit (JDK 8 or higher) installed and configured in your system environment.

### Compilation
Open your terminal/PowerShell inside the project root folder (ensure you are inside the directory containing the `graph` package structure) and run:
```bash
javac graph/Graph.java
```

### Execution
Run the compiled bytecode using the following command:
```bash
java graph.Graph
```
*(Note: Ensure `res.txt` is present in the root execution directory, as it contains the default target graph for the `main` method execution loop).*

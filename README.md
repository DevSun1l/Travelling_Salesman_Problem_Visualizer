# Travelling_Salesman_Problem_Visualizer

An interactive, high-fidelity pedagogical tool designed to teach the complexities of the **Traveling Salesperson Problem (TSP)**, **NP-Completeness**, and **Algorithmic Heuristics**.

This visualizer allows students to explore how different algorithms navigate the NP-Hard challenge of finding the shortest possible route that visits every city and returns to the origin.

## 🛠️ Key Features

### 1. Interactive Map Visualizer
- **Unidirectional Paths**: Real-time rendering of the tour with directional arrows showing the salesperson's flow.
- **Live Edge Costs**: Dynamic distance labels displayed directly on the map for every connection.
- **State Highlighting**: Color-coded visualization (Blue for current traversal, Green for optimal results, Orange for candidate swaps).

### 2. Algorithmic Engines
- **Brute Force (Exact)**: Evaluates every possible permutation ($O(n!)$). Demonstrates the "Combinatorial Explosion" and why exact solutions are impossible for large datasets.
- **Nearest Neighbor (Greedy)**: A fast heuristic ($O(n^2)$) that always picks the closest unvisited city. Demonstrates how local "short-term" choices can lead to poor global results.
- **2-Opt Local Search**: An improvement heuristic that "untangles" route crossings to optimize a tour. Shows the power of iterative improvement.

### 3. Interactive Learning System
- **Synced Pseudocode**: Real-time highlighting of code lines as the simulation runs. Click any line for a deep-dive mathematical explanation.
- **Simulation Time-Machine**: Full "Undo/Redo" capabilities with **Prev Step**, **Next Step**, and **Skip to End** buttons.
- **Theory Guide**: Integrated reduction proof showing how a **Hamiltonian Cycle** instance transforms into a TSP problem with a budget constraint.
- **Complexity Curves**: Interactive SVG chart comparing the growth of $O(n!)$ vs $O(n^2)$.

### 4. Comparison & Analysis
- **Compare Mode**: Run **Greedy vs 2-Opt** simultaneously on the same map to compare accuracy (Tour Quality) vs Computation Time.
- **Real-World Context**: Integrated case studies on Logistics, Manufacturing (PCB Drilling), and Genetics (DNA Sequencing).

## 🚀 Getting Started

The entire application is self-contained in a single file for maximum portability.

1. Navigate to the project directory.
2. Open `tsp.html` in any modern web browser (Chrome, Firefox, Edge, Safari).
3. Click **Generate Graph** to start.

## 🧪 Technical Details
- **Core**: HTML5 / Vanilla JavaScript (ES6+).
- **Styling**: Modern CSS3 with Glassmorphism and CSS Variables.
- **Logic**: Native **JavaScript Generators** (`async*`) for non-blocking UI updates and step-by-step state management.
- **Graphics**: SVG (Scalable Vector Graphics) for the coordinate-based map and complexity charts.



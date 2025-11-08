# Air-Traffic-Control---Kruskal-Dijkstra-DAA-
The project, “Air Traffic Control System using Kruskal’s and Dijkstra’s Algorithms,” is a Python-based software solution that demonstrates the use of two classical graph algorithms Kruskal’s Minimum Spanning Tree Algorithm and Dijkstra’s Shortest Path Algorithm for efficient route optimization in an air traffic control network.

The development of the Air Traffic Control System using Kruskal’s and Dijkstra’s Algorithms was carried out through a structured and modular approach. Each phase of the implementation focused on building one core component of the system — ensuring algorithmic accuracy, interface usability, and efficient data handling. The following steps outline the entire development process:

Step 1: Requirement Analysis
The project began with the identification of core functional and non-functional requirements. The main objective was to develop an interactive desktop application that demonstrates how Kruskal’s and Dijkstra’s algorithms can be used for air route optimization.
Key requirements included:
•	A graphical interface for data input and algorithm execution.
•	Support for dynamic graph creation using vertices and edges.
•	Accurate implementation of both algorithms with efficient output display.
•	A simple, educational interface suitable for students and researchers.

Step 2: Algorithm Design
Two algorithms were designed as separate modules within the project:
•	Kruskal’s Algorithm: Used to construct the Minimum Spanning Tree (MST), connecting all airports (vertices) with the least total route cost.
•	Dijkstra’s Algorithm: Used to find the shortest path from a selected source airport to all other airports.
Both algorithms were designed using object-oriented programming (OOP) principles to ensure modularity and ease of integration with the GUI.

•	Step 3: Graph Input and Data Handling
The system allows users to dynamically create graphs by entering the number of vertices (airports) and weighted edges (routes with distances or costs). Each edge input is validated to ensure:
•	Non-negative weights (distances).
•	Vertices within valid range.
•	Avoidance of duplicate or self-loop connections.
The edges are temporarily stored in an internal list structure, which is then processed by the selected algorithm.

Step 4: GUI Design using Tkinter
The graphical user interface was developed using Tkinter, Python’s standard GUI library. It includes:
•	Vertex Input Section: For setting the total number of airports.
•	Edge Input Section: For entering air routes in the format (u, v, weight).
•	Algorithm Buttons: For executing Kruskal’s and Dijkstra’s algorithms independently.
•	Output Display: A text box that displays MST edges, total cost, or shortest path distances.
The interface was designed to be simple and interactive, ensuring that users can easily visualize the algorithms’ outputs.

Step 5: Kruskal’s Algorithm Implementation
The Kruskal class was implemented with the following functions:
•	add_edge(u, v, w): Adds an edge to the graph.
•	find(parent, i): Identifies the parent of a node for the disjoint-set operation.
•	union(parent, rank, x, y): Merges two subsets during MST construction.
•	kruskal_mst(): Sorts edges by weight, selects edges that do not form cycles, and constructs the Minimum Spanning Tree.
The output displays all selected edges and the total cost of the MST, demonstrating the concept of connecting all nodes with minimal cost.

Step 6: Dijkstra’s Algorithm Implementation
The Dijkstra class includes:
•	A matrix-based graph representation for efficient path computation.
•	add_edge(u, v, w) for establishing weighted connections.
•	min_distance() for selecting the nearest unvisited vertex.
•	dijkstra(src) for calculating the shortest distance from the source to all other nodes.
The results display each vertex along with its shortest distance from the chosen source airport.

Step 7: Integration and Testing
After implementing both algorithms separately, the components were integrated into a single Tkinter application. The system was tested for:
•	Input validation and user errors.
•	Correctness of MST and shortest path results.
•	Stability and responsiveness of the GUI.
Various test cases were used, including small and medium-sized graphs, to confirm that both algorithms produced accurate and consistent outputs.

Step 8: Output Visualization and Evaluation
The final stage involved testing the readability and accuracy of the displayed results. The text output was formatted clearly to show:
•	All edges included in the MST with their weights and total cost.
•	Shortest paths from the source vertex to all destinations.
Through repeated evaluations, the system demonstrated its ability to efficiently compute optimal connections and paths while maintaining an intuitive interface.

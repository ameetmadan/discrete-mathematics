# Graphs

Graphs are a powerful problem-solving tool because they enable us to represent a complex situation with a single image that can be analyzed both visually and with the aid of a computer

## Terminology of graphs

- Graph: The whole drawing
- Parallell edges: 2 edges connecting to each other
- Isolated vertex: No edges connected
- Adjaceny: 2 connected edges
- Degree: Number of edges that start or end at a vertex

![](26_05_2021_16.39.png)

![](26_05_2021_16.30.png)

## Sub-graphs

The left graph has 11 sub-graphs

![](26_05_2021_16.33.png)

## Matrices and directed graphs

Show connections from vertices to other vertices in form of a matrix

![](26_05_2021_16.46.png)

## Matrices and undirected graphs

Note that an adjacency matrix of an undirected graph is symmetric.

![](26_05_2021_17.07.png)

## Matrices and connected components

![](26_05_2021_17.12.png)

The adjacency matrix of this graph is a block-diagonal matrix: it consists of square matrix blocks for each connected component, along the diagonal, and blocks of 0’s everywhere else. The reason is that vertices in each connected component share no edges with vertices in other components.

## Isomorphisms of graphs

Two graphs that are the same except for the labeling of their vertices and edges are called isomorphic

![](26_05_2021_17.16.png)

The first two graphs are identical althought their topology is different: their vertex and edge sets are identical and their edge-endpoint functions are the same.

# Trails

Trails are routes that do not have a repeated edge.

![](26_05_2021_17.17.png)

Not a trail: 

![](26_05_2021_17.18.png)  

# Paths

Paths are trails that do not have repeated vertices

Without the loop on $v_3$ this would be a path

![](26_05_2021_17.17.png)


# Circuits

Circuits are trails that start and end at the same vertex

![ ](26_05_2021_17.26.png)  

## Simple circuits

Simple circuits are circuits that only pass through each vertex of the circuit only once, except for the start and end vertices

![](26_05_2021_17.27.png)  

## Euler cicuits

An Euler circuit passes through all the vertices of G at least once and passes through all the edges only once.

![](26_05_2021_17.31.png)

A graph has an Euler circuit if, and only if, the graph is connected and every vertex of the graph has even degree (because the total number of arrivals and departures from each vertex must be a multiple of 2).

## Hamiltonian circuits

A Hamiltonian circuit for a graph G is a circuit that passes through all the vertices of G only once (except for the start and end vertices). Since it is a circuit, it has no repeated edges.



## Example: Travelling salesman problem

# Trees

## Rooted trees

## Binary trees

## Octrees

## Spanning trees

### Minimum spanning trees

# Kruksal's Algorithm

# Prim's Algorithm

# Dijkstra's Algorithm
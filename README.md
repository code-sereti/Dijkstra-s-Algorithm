# Dijkstra-s-Algorithm
It computes the shortest distance from a given vertex to the rest of the vertices in a graph

Dijkstra’s Algorithm works like the following:

Instantiate a dictionary that will eventually map vertices to their distance from the start vertex
Assign the start vertex a distance of 0 in a min heap
Assign every other vertex a distance of infinity in a min heap
Remove the vertex with the smallest distance from the min heap and set that to the current vertex
For the current vertex, consider all of its adjacent vertices and calculate the distance to them as (distance to the current vertex) + (edge weight of current vertex to adjacent vertex).
If this new distance is less than the current distance, replace the current distance.
Repeat 4 and 5 until the heap is empty
After the heap is empty, return the distances

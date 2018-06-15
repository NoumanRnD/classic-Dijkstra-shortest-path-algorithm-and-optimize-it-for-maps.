# classic-Dijkstra-shortest-path-algorithm-and-optimize-it-for-maps.
Implement the classic Dijkstra  shortest path algorithm and
optimize it for maps. Such algorithms are widely used in
geographic information systems (GIS) including MapQuest and
For example, input.txt represents the map below:<br/>
GPS-based car navigation systems.<br/><br/>
Maps. For this assignment we will be working with maps, or
graphs whose vertices are points in the plane and are connected by
edges whose weights are Euclidean distances. Think of the vertices
as cities and the edges as roads connected to them. To represent a
map in a file, we list the number of vertices and edges, then list the
vertices (index followed by its x and y coordinates), then list the edges (pairs of vertices), and finally the source and sink vertices.
 <br/><br/>
#Dijkstra algorithm.<br/><br/> 
Dijkstra  algorithm is a classic solution to the
 
shortest path problem. The basic idea is not difficult to understand.
We maintain, for every vertex in the graph, the length of the
shortest known path from the source to that vertex, and we
For example, input.txt represents the map below:<br/><br/>
maintain these lengths in a priority queue. Initially, we put all the
vertices on the queue with an artificially high priority and then
assign priority 0.0 to the source. The algorithm proceeds by taking
the lowest-priority vertex off the PQ, then checking all the vertices
that can be reached from that vertex by one edge to see whether
that edge gives a shorter path to the vertex from the source than the
shortest previously-known path. If so, it lowers the priority to
reflect this new information.

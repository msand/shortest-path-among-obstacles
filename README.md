The starting and end points as well as the polygon obstacles are read from the files points.xml and polygons.xml. It is important to
list polygon points in a clockwise or counterclockwise direction (in a consecutive order). The algorithm is run in three stages, 
the first one is calculating the visibility graph. After that, clicking on a point will highlight all other points visible from it.
The second stage is adding weight to edges in the visibility graph, every edge will have a weight corresponding to the Euclidean distance
between the points it connects. The third and final stage is calculating the shortest path between the start and end point using
Dijsktra'a algorithm.
Graff is a Node.JS graph theory library with some utility functions. At some
point, persistence backends may be added, but for the time being it just runs in
memory.

Not much is supported right now. You can add vertices, connect them, disconnect
them, and find the shortest path between two nodes (if it exists). Dijkstra's
algorithm is used unless Graph.uniform is true (false by default), in which case
a more efficient uniform cost search implementation is used. If you set
Graph.directed to false (true by default), then edges will be considered
undirected for the sake of path finding.

See lib/test.js for examples. This file isn't a real test suite, just a useful
file that sped up some testing during development.
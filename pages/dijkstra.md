# dijkstra

> Compute shortest-path distances from a single source node in a graph.
> More information: <https://graphviz.org/pdf/dijkstra.1.pdf>.

- Compute distances from a given source node in a graph file:

`dijkstra {{source_node_file}}`

- Treat the graph as directed when computing distances:

`dijkstra -d {{source_node_file}}`

- Record the previous closest node for each node on the shortest path:

`dijkstra -p {{source_node_file}}`

- assign large distance values to unreachable nodes:

`dijkstra -a {{source_node_file}}`

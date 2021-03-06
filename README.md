![](https://github.com/ShalevAsor/Ex3/blob/master/data/directed1.png)

## What is directed weighted graph? <br>
simple graph made up of vetices and edges. <br>
the difference btween simple unweighted graph to weighted graph <br>
is that each edge on a weight graph has weight wich is a positive number. <br>
the difference between directed graph to simple undirected graph is that <br>
each edge in direceted graph has a direction. <br>
edge between node 1 and node 2 is NOT equals to edge between node 2 to node 1. <br>
you can find much more information about directed graph [here](https://en.wikipedia.org/wiki/Directed_graph) <br>



## The benefits of using GraphAlgo:
- Low Complexity
- Support more than one mil verteices and ten mil edges
- each public class has tests
- support algorithms like Dijkstra's and Bfs
- each un-trivail metohd attached with explanations
- support ploting the graph and create randomly positions 
- quick access to nodes/edges 
To see the comparison with other graphs click [here](https://github.com/ShalevAsor/Ex3/wiki) <br>
 

## How it works? 
add node into the graph : add_node(<node id>, <position>) <br>
connect two nodes with a weight: add_edge(<source node key >,<destination node key>, <weight>) <br>
remove node from the graph: remove_node(<node key>) <br>
Note: this method will remove all the edges that this node was associate with <br>
remove edge from the graph: remove_edge(<node src key>,<node dest key>) <br>
dictunary of all the nodes in the graph : get_all_v() <br>
dictunary of all the node that connected **to** the node_id : all_in_edges_of_node(<node_id>) <br>
 dictunary of all the node that connected  **from** the node_id : all_out_edges_of_node(<node_id>) <br>
For more information, i recommend diving into the code, there is explanations attached to each method. <br>
 
 
## GraphAlgo

This class supports few algorithms like dfs tarjan and dijkstra's <br>
it allows to save the graph into a json format and load a graph from json format <br>
the dfs and tarjan algo used to find out if this graph is strongly connected and the connected commponents <br>
**methods:** <br>
- **connected_components:** return all the strongly connected commponents in the graph <br>
**what is strongly connected graph ?** <br>
it means there is a path from each node in the graph to every other node <br>
for example: <br>
this graph is **Not strongly connected** <br>
![](https://github.com/ShalevAsor/Ex3/blob/master/data/dir2.png) <br>

this graph is **strongly connected** <br>
![](https://github.com/ShalevAsor/Ex3/blob/master/data/dir.png)

for more information about strongly connected graph : click [here](https://en.wikipedia.org/wiki/Strongly_connected_component) <br>

dijkstra's algorithm used in the methods shortest_path <br>
- **Shortest path:** return the shortest path between two nodes in the graph and the length of the path. <br>
the shortest path will be the path with the minimalist edges weight <br>
for example : <br>
<a href="http://www.siz.co.il/"><img src="http://up419.siz.co.il/up2/2mdhzomitddn.png" border="0" alt="shortest" /></a> <br>
the shortest path from node 1 to 2 is : 1---> 3--->2 <br>

- **plot_garph:** plot the graph - if the vertices has no positions the will be places in randomly (elegant) <br>
**example:** <br>
![](https://github.com/ShalevAsor/Ex3/blob/master/data/random_graph_example.png)


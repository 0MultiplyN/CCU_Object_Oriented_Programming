# CCU_Object-Oriented Programming
## Functionality of this code
1. Provides C++ classes for simulating elements in network communication, such as headers, data, packets, nodes, events, and links.
2. Implements packet routing functionality using the shortest path algorithm to calculate distances between nodes and the next-hop path.
3. Allows simulation of different network topologies and communication protocols by modifying the links and weights between nodes.
### About Shortest path algorithm
- using Floyd-Warshall algorithm
### Procedure
- In this code, the routing functionality is implemented using the Floyd-Warshall algorithm. This algorithm is a dynamic programming algorithm used to compute the shortest paths between all pairs of nodes in a graph. In the implementation, the distance matrix between nodes is first initialized. 
- Then, a triple loop is used to update the distance matrix until all the shortest paths between nodes are computed. During the updating process, if a shorter path is found for a certain pair of nodes, the distance matrix and the next-hop matrix are updated accordingly. 
- Finally, the next-hop matrix can be used to implement the packet forwarding functionality, which involves looking up the next-hop node ID based on the destination node ID until the packet reaches its destination node.
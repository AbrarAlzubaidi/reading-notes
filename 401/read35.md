# Graphs
graphs is a non-linear DS similar of trees

contains:
1. nodes/ vertices
2. edges: to connect each node with another node/nodes

![grahs](https://www.upgrad.com/blog/wp-content/uploads/2020/10/1.png)

## graph types
1. directed

each node connect with others with directed edge which means there is one way to traverse

Ex: in below example

    - node A traverse to B only
    - node B traverse to D only
    - node C traverse to E only
    - node D traverse to A only
    - node E traverse to D only


![directed-graph](https://static.javatpoint.com/ds/images/directed-and-undirected-graph.png)


-----

2. un-directed

each node connect with others with un-directed edge which means there are many ways to traverse between 2 connected nodes

Ex: in below example

    - node A traverse to B and E
    - node B traverse to D and C
    - node C traverse to B and D
    - node D traverse to B and E
    - node E traverse to D and A

![un-directed-graph](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQpvmPgGqDGdJbEfaxiGbEp_TYjrHyDU5XSkw&usqp=CAU)


----

3. weighted

each edge has a weight/ value
this weight will consider when you traverse from nodes 
<p style='color:#064663'><b>
(you can imagin it as a distance between 2 cities so if i want to move from city A to city B i am going to take the shortest path ^^)
</b>
</p>

![weighted-graph](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ0-nsjVmmq5H_akQ3HtLuEt4luevb5R1UFuusVcCDNuTl6251hbcOIGrK9MYhk1P7c6Xo&usqp=CAU)

4. un-weighted

each edge does not have a weight/ value
 
<p style='color:#064663'><b>
(it is like a normal graph ^^)
</b>
</p>


![un-weighted-graph](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQpvmPgGqDGdJbEfaxiGbEp_TYjrHyDU5XSkw&usqp=CAU)


## Complete vs Connected vs Disconnected

1. complete:

A complete graph is when all nodes are connected to all other nodes

![complete-graph vs not-complete-graph](https://codefellows.github.io/common_curriculum/data_structures_and_algorithms/Code_401/class-35/resources/assets/CompleteGraph.PNG)

2. connected vs dis-connected

<b style='color:#E5890A'>A connected graph </b>is graph that has all of nodes have at least one edge.

<b style='color:#E5890A'>A disconnected graph </b>is a graph where some vertices may not have edges.

![connected vs dis-connected graph](https://i2.wp.com/techvidvan.com/tutorials/wp-content/uploads/sites/2/2021/07/TV-DS-Graph-normal-image06.jpg?w=656&ssl=1)


## Adjacency Matrix
An Adjacency matrix is represented through a 2-dimensional array. If there are n vertices, then we are looking at an n x n Boolean matrix

- The elements of both the column and the row must add up to 1 if there is an edge that connects the two, or zero if there isn’t a connection.

![Adjacency Matrix](https://pythonandr.files.wordpress.com/2016/07/adjacencymatrix.png?w=700)


## Adjacency List

An adjacency list is a collection of linked lists or array that lists all of the other vertices that are connected.

![Adjacency List](https://kajabi-storefronts-production.kajabi-cdn.com/kajabi-storefronts-production/blogs/27029/images/FVKdPFTlTmyXQBiypTge_375dbebabc31445637557c91ec1fe4de.jpg)


## so HOW to Traverse graph?

1. **Breadth First Algorithm**


        ALGORITHM BreadthFirst(vertex)
            DECLARE nodes <-- new List()
            DECLARE breadth <-- new Queue()
            DECLARE visited <-- new Set()

        breadth.Enqueue(vertex)
        visited.Add(vertex)

        while (breadth is not empty)
            DECLARE front <-- breadth.Dequeue()
            nodes.Add(front)

            for each child in front.Children
                if(child is not visited)
                    visited.Add(child)
                    breadth.Enqueue(child)   

        return nodes;

2. **Depth First Algorithm**

        procedure DFS_iterative(G, v) is
            let S be a stack
            S.push(iterator of G.adjacentEdges(v))
            while S is not empty do
                if S.peek().hasNext() then
                    w = S.peek().next()
                    if w is not labeled as discovered then
                        label w as discovered
                        S.push(iterator of G.adjacentEdges(w))
                else
                    S.pop()
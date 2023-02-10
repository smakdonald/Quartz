#### $\defn$ – 
A *graph* $G$ is a set of *vertices* $V (G)$, a set of *edges* $E(G)$, and a relation that associates  
with each edge two vertices called its endpoints.  
#### $\defn$ – 
A *loop* is an edge whose endpoints are the same.  
#### $\defn$ – 
*Multiple edges* are edges with the same endpoints.  
#### $\defn$ – 
A *simple graph* is a graph with no loops or multiple edges.  
#### $\defn$ – 
Two vertices v and w in G are *adjacent*, denoted v ↔ w, if there is an edge between  
them.  
#### $\defn$ – 
If the vertex v is an endpoint of the edge e, then e and v are *incident*.  
#### $\defn$ – 
The *degree* $d(v)$ of a vertex $v$ is the number of edges incident to it, counting loops  
twice.  
#### $\defn$ – 
An *isomorphism* between two simple graphs G and H is a bijection φ : V (G) →  
V (H) such that vw ∈ E(G) if and only if φ(v)φ(w) ∈ E(H).  
Two graphs are *isomorphic* if there exists an isomorphism between them.  
#### $\defn$ – 
The *complement* of a simple graph G is the graph G with V (G) = V (G), and  
uv ∈ E(G) if and only if uv 6 ∈ E(G).  
#### $\defn$ – 
The *path* Pn is the graph with n vertices v1, . . . , vn and edges v1v2, . . . , vn−1vn.  
#### $\defn$ – 
The *cycle* Cn is the graph with n vertices v1, . . . , vn and edges v1v2, . . . , vn−1vn, vnv 
#### $\defn$ – 
The *complete graph* Kn is the graph with n vertices in which every pair of vertices  
are adjacent.  
#### $\defn$ – 
A graph G is *bipartite* if its vertices can be partitioned into two sets X and Y , called  
partite sets, such that every edge in E(G) is between a vertex in X and a vertex in  
Y .  
#### $\defn$ – 
The *complete bipartite* graph Km,n is the bipartite graph with partite sets of m  
vertices and n vertices, such that every pair of vertices in different sets are adjacent.  
#### $\defn$ – 
The *adjacency matrix* A of a graph G with n vertices is the n × n matrix with rows  
and columns indexed by the vertices of G, where the number in the ith row and jth  
column of A is the number of edges between the ith and jth vertex, counting loops  
twice.  
#### $\defn$ – 
The *incidence matrix* M of a graph G with n vertices and e edges is the n × e  
matrix with rows indexed by the vertices of G and columns indexed by the edges of G,  
where the number in the ith row and jth column of A is the number of times vertex i  
and edge j are incident, counting loops twice.  
#### $\defn$ – 
A *walk* in a graph is an alternating sequence of vertices and edges v1e1v2e2...vkek, such  
that each term of the sequence is incident to the next.  
#### $\defn$ – 
A *trail* is a walk with no repeated edge.  
#### $\defn$ – 
A *path* is a walk with no repeated vertex.  
#### $\defn$ – 
A *circuit* is a trail whose first and last vertices are the same.  
#### $\defn$ – 
A *cycle* is a circuit with no repeated vertex other than the first and last vertex.  
#### $\defn$ – 
The *length* of a walk, trail, path, circuit, or cycle in a graph is the number of edges  
in it (counting repeated edges multiple times).  
#### $\defn$ – 
The *girth* of a graph G is the length of its shortest cycle. If G has no cycles, then its  
girth is infinite.  
#### $\defn$ – 
A graph G is *connected* if, for every pair of vertices in G, there exists a path between  
them.  
#### $\defn$ – 
A *component* of a graph G is a maximal connected subgraph of G.  
#### $\defn$ – 
A *cut edge* or *cut vertex* of a graph G is an edge or vertex whose deletion increases  
the number of components of G.  
#### $\defn$ – 
A *subgraph* H of a graph G is a graph such that V (H) ⊆ V (G) and E(H) ⊆ E(G).  
#### $\defn$ – 
An *induced subgraph* H of a graph G is a subgraph of G obtained by deleting a set  
of vertices.  
#### $\defn$ – 
An *Eulerian circuit* (alternatively, Euler tour ) of a graph G is a circuit which  
contains every edge of G.  
#### $\defn$ – 
A graph is *Eulerian* if it contains an Eulerian circuit.  
#### $\defn$ – 
A *Hamiltonian cycle* of a graph G is a cycle which contains every vertex of G.  
#### $\defn$ – 
A graph is *Hamiltonian* if it contains a Hamiltonian cycle.  
#### $\defn$ – 
A graph G is *regular* if every vertex of G has the same degree. If that degree is k,  
then G is k-regular.  
#### $\defn$ – 
The *neighborhood* of a vertex v is the set of vertices adjacent to v.  
#### $\defn$ – 
The *degree sequence* of a graph is the list of degrees of the graph, in non-increasing  
order.  
#### $\defn$ – 
A *tree* is a connected graph with no cycles.  
#### $\defn$ – 
A *leaf* of a tree is a vertex of degree  
#### $\defn$ – 
A *spanning subgraph* H of a graph G is a subgraph of G such that V (H) = V (G).  
#### $\defn$ – 
A *spanning tree* of a graph G is a spanning subgraph of G which is a tree.  
#### $\defn$ – 
The *distance* d(v, w) between two vertices v and w is the length of the shortest path  
between them.  
#### $\defn$ – 
The *diameter* of a graph G is the largest distance between any pair of vertices. If G  
is disconnected, then its diameter is infinite.  
#### $\defn$ – 
A *forest* is a graph with no cycles.  
#### $\defn$ – 
A *directed graph* or digraph G is a set of vertices V (G), a set of edges E(G), and a  
relation that associates with each edge an ordered pair of vertices called its endpoints.  
The first vertex in the ordered pair is the tail and the second vertex is the head of  
the edge.  
#### $\defn$ – 
If G is a directed graph, the *underlying graph* of G is the graph obtained from G  
by un-ordering each of its edges.  
#### $\defn$ – 
If G is a graph, an *orientation* of G is obtained from G by ordering each of its edges.  
#### $\defn$ – 
A *tournament* is an orientation of a complete graph.  
#### $\defn$ – 
The *indegree* d−(v) of a vertex v is the number of edges with head v. The *outdegree*  
d+(v) of a vertex v is the number of edges with tail v.  
#### $\defn$ – 
A *directed walk* in a graph is an alternating sequence of vertices and edges v1e1v2e2...vkek,  
such that ei = vivi+1 for all 1 ≤ i ≤ k −  
#### $\defn$ – 
A directed graph G is *strongly connected* if there is a directed path from every  
vertex to every other vertex in G.  
#### $\defn$ – 
A directed graph is *weakly connected* if its underlying graph is connected.  
#### $\defn$ – 
A directed graph is *acyclic* if it contains no directed cycles.  
#### $\defn$ – 
A directed graph G is *transitive* if (x, y), (y, z) ∈ E(G) implies (x, z) ∈ E(G) for all  
x, y, z ∈ V (G).  
#### $\defn$ – 
A *matching* in a graph is a set of edges with no shared endpoints.  
#### $\defn$ – 
A matching is *perfect* if its edges are incident to every vertex in G.  
#### $\defn$ – 
An *independent set* of a graph G is a set of pairwise non-adjacent vertices.  
#### $\defn$ – 
The *independence number* α(G) is the maximum size of an independent set in G.  
#### $\defn$ – 
A *vertex cover* of G is a set of vertices S such that every edge of G is incident to  
some vertex in S.  
#### $\defn$ – 
An *edge cover* of G is a set of edges S such that every vertex of G is incident to some  
edge in S.  
#### $\defn$ – 
A *vertex cut* of a graph G is a set of vertices S of G such that G − S is disconnected. 
#### $\defn$ – 
A graph is k-*connected* if it has no vertex cut with fewer than k vertices.  
#### $\defn$ – 
A graph has *connectivity* k, denoted κ(G), if it is k-connected and not (k + 1)-  
connected.  
#### $\defn$ – 
A *block* of a graph G is a maximal connected subgraph of G with no cut vertices.  
#### $\defn$ – 
An *edge cut* of a graph G is a set of edges S of G such that G − S is disconnected.  
#### $\defn$ – 
A graph is k-*edge-connected* if it has no edge cut with fewer than k edges.  
#### $\defn$ – 
A graph has *edge-connectivity* k, denoted κ′(G), if it is k-edge-connected and not  
(k + 1)-edge-connected.  
#### $\defn$ – 
A k-*coloring* of a graph G is an assignment of k colors to the vertices of G.  
#### $\defn$ – 
A coloring is *proper* if adjacent vertices receive distinct colors.  
#### $\defn$ – 
A graph G is k-*colorable* if it has a proper k-coloring.  
#### $\defn$ – 
The *chromatic number* χ(G) is the least k such that G is k-colorable.  
#### $\defn$ – 
A graph G is *color critical* or k-critical if χ(H) < χ(G) for every proper subgraph  
H of G.  
#### $\defn$ – 
A *clique* in a graph G is a complete induced subgraph of G.  
#### $\defn$ – 
The *clique number* ω(G) is the maximum size of a clique in G.  
#### $\defn$ – 
A graph is k-*partite* if its vertices can be partitioned into k independent sets.  
#### $\defn$ – 
If G is a graph and xy is an edge of G, we *subdivide* the edge xy by adding the vertex  
z and replacing the edge xy by the two edges xz and zy.  
#### $\defn$ – 
A *subdivision* of a graph G is a graph that can be obtained from G by a sequence of  
edge subdivisions.  
#### $\defn$ – 
If G is a graph and e = xy is an edge of G, we *contract* e, denoted by G·e, by deleting  
e and identifying the vertices x and y.  
#### $\defn$ – 
A *minor* of a graph G is a graph that can be obtained from G by a sequence of edge  
deletions and contractions.  
#### $\defn$ – 
The *join* of two graphs G and H, denoted G ∨ H, is the graph with vertex set V (G) ∪  
V (H) and edge set E(G) ∪ E(H) ∪ {xy | x ∈ V (G), y ∈ V (H)}.  
#### $\defn$ – 
The *Cartesian product* of two graphs G and H, denoted GH, is the graph with  
vertex set V (G) × V (H) and edge set {(u, v)(u′, v′) | u = u′ and vv′ ∈ E(H) or v =  
v′ and uu′ ∈ E(G)}.  
#### $\defn$ – 
The *chromatic polynomial* χ(G; k) of the graph G is the function which takes any  
positive integer k and returns the number of proper k-colorings of G.  
#### $\defn$ – 
A graph is *planar* if it can be drawn in the plane with no edge-crossings.  
#### $\defn$ – 
A drawing of a planar graph in the plane with no edge-crossings is called a *planar  
embedding* of G or a plane graph.  
#### $\defn$ – 
A *face* of a plane graph G is a maximal connected subset of R2 − G.
#### $\defn$ – 
Two faces of a plane graph are *adjacent* if they share an edge.  
#### $\defn$ – 
The *dual* G∗ of a plane graph G is the graph with vertex set equal to the face set of  
G, and with an edge between two vertices for each edge between their corresponding  
faces
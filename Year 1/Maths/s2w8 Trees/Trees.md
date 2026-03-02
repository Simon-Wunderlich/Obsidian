Created: Oct 05 2025
Class: [[Trees]] 
- - -
# Tree definition
Acyclic
Undirected
Connected
Corrected [[Directed acyclic graph]]
$Num \space edges = num \space verticies - 1$
$Num \space leaves \geq 2$ if more than 1 node
$\chi(G) = 2$
# Tree types
Types of rearranging the same trees
## Free
![[Pasted image 20251005140018.png]]
## Rooted
![[Pasted image 20251005140028.png]]

# Terminology
## Level
The number of edges between vertex and root
## Height
Highest level in tree
## Parent
Vertex connected to node with a higher level
## Child
Vertex connected to node with lower level
## Siblings
Two vertexes with the same parent
## Ancestors
Every vertex with transitive closure to a node with higher level
## Descendant
Node $a$ is a descendant of node $b$ if $b$ is an ancestor of $a$
## Leaf
Vertex with no children
## Subtree
Tree containing node $v$ and all descendants of $v$ who's edges are all in original graph
## Internal vertex
Vertex with degree of at least 2

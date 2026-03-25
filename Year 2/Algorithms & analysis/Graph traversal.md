Created: Mar 25 2026
Class: [[Algorithms & analysis]] 
- - -

## Search tree
Show graph reshaped as tree by the traversal of the algorithm. 
Remove all unvisited edges. - Tree by definition.
Use start node as root
## Account for disconnected components
```python
VISITED = []
V = [] # Set of all nodes
for x in V:
	if x not in VISITED:
		# Do D/BFS with x as root
```


# DFS
## Pop order
List in which nodes are popped (Topological sort)
## Push order
List in which nodes are pushed (Traversal order)
# BFS
## Enqueue order
List in which nodes are enqueued (traversal order)
## Dequeue order
Same as enqueue order

Created: Oct 08 2025
Class: [[Trees]] 
- - -
# Hash
One way function (irreversible)
Converts any data into fixed length "Hash" deterministically. 
Similar inputs outputs vastly different hashes

# Merkle Trees
![[Pasted image 20251008110456.png]]
At each level of the merkle tree, each node hashes the concatenation of its children
Merkle root represents digital signature of entire tree. Will change dramatically should any input slightly change

# Data synchronisation
To compare two databases to determine in which records they differ
1. Run both databases through Merkle tree, with each record as a leaf
2. Traverse through both Merkle trees from root. (DFS)
	- Compare all hashes at current level
	- Traverse to branch in which hashes do not match
$$O(ln(n))$$

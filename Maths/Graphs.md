Created: May 15 2025
Class: [[Maths]] 
- - -
### Binary relations
Basically same concept as unweighted digraph, same as adjacency matrix

### Syntax
For a binary relation $R$ of a set $A$, a connection between elements $x$ and $y$ is described as
$$
xRy
$$
$$
x,y\in A
$$

### Reflexive binary relations
**All elements are connected to themselves**, where $R$ is a binary relation of set $A$.
$$
\forall x, \space xRx
$$
![[Pasted image 20250515140806.png]]
### Anti-Reflexive binary relations
**No elements are connected to themselves**, where $R$ is a binary relation of set $A$.
$$
\forall x, \space xRx \space does \space not \space exist
$$
![[Pasted image 20250515140825.png]]
### Symmetric binary relations
Each pair of elements $x$ and $y$ with an edge (x,y) also has an edge (y,x)
$$
\forall x \forall y, \space xRy \leftrightarrow yRx
$$
ie
$$
\forall x \space and \space y \in A: xRy \cap yRx
$$
![[Pasted image 20250515140840.png]]
### Anti-symmetric relations
Each pair of elements $x$ and $y$ with an edge (x,y) cannot have an edge (y,x), given that x$\neq$y
$$
\forall x \forall y, \space xRy \space \leftrightarrow \space \neg yRx
$$
ie
$$
\forall x \space and \space y \in A: \neg(xRy \cap yRx) 
$$
![[Pasted image 20250515140852.png]]

### Transitive relations
$$\forall x \forall y \forall z, \space (xRy \space and \space yRx) \rightarrow xRz$$
![[Pasted image 20250516101947.png]]

![[Types of walks]]

![[Compositions of relations]]
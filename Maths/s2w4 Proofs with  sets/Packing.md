Created: Sep 05 2025
Class: [[Maths]] 
- - -
# Unpacking
Remove an operator while maintaining logical equivalence
## Complement
$$
(x \in \bar{X}) \rightarrow (x \not \in X)
$$
## Union
$$
(x \in X \space \cup \space Y) \rightarrow (x \in X \space or \space x \in Y)
$$
## Intersection
$$
(x \in X \space \cap \space Y) \rightarrow (x \in X \space and \space x \in Y)
$$
## Set difference
$$
(x \in X-Y) \rightarrow (x \in X \space and \space x \not \in Y)
$$
## Symmetric difference
$$
(x \in X \oplus Y) \rightarrow (x \in X \space and \space x \not \in Y) \space or \space (x \not \in X \space and \space x \in Y)
$$

# Repacking
Introduce an operator while maintaining logical equivalence.
## Complement
$$
(x \in X) \rightarrow (x \not \in  \bar{X})
$$
## Union
$$
 (x \in X \space or \space x \in Y) \rightarrow (x \in X \space \cup \space Y)
$$
## Intersection
$$
(x \in X \space and \space x \in Y) \rightarrow (x \in X \space \cap \space Y)
$$
## Set difference
$$
 (x \not \in X \space or \space x \in Y) \rightarrow (x \in X-Y)
$$
## Symmetric difference
$$
(x \in X \space and \space x \not \in Y) \space or \space (x \not \in X \space and \space x \in Y) \rightarrow (x \in X \oplus Y) 
$$
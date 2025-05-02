Created: Apr 14 2025
Class: [[Maths]] 
- - -
### Combinations
To count the number of possible pairings from sets $A$ and $B$
$$
|A \times B|
$$
### Permutations
Ordered
$$P(n,r) = \frac{n!}{(n-r)!}$$
$$= n\cdot(n-1)\cdot(n-2)\cdots(n-(r-1))$$
#### $$\prod\limits^{n}_{k=n-(r-1)}k$$
$$n \space choose \space r$$
### Counting subsets
Order doesn't matter for subsets
Divide by r! as r! represents the amt of ways to reorder a set of r elements
$$\# \space of \space r-subsets \space from\space  S=C(n,r)=
\begin{pmatrix}
           n\\
           r
         \end{pmatrix}=\frac{P(n,r)}{r!}$$
$$=\frac{n!}{r!(n-r)!}$$
$$=\begin{pmatrix}n \\ r\end{pmatrix}$$
$$\frac{n \cdot (n-1) \cdots (n-r+1)}{r!}$$
#### $$\frac{\prod\limits^{n}_{k=n-(r-1)}k}{r!}$$
### Counting permutations with repetitions
The number of permutations of set {a, b, a , a, c} with $n_a$ a's, $n_b$ b's, $n_c$ c's where $n = n_a+n_b+n_c$

$$
\frac{n!}{n_a! \cdot n_b! \cdot n_c!}
$$
ie
$$
\frac{totalLengthOfSet!}{numberOfAs!\cdot numberOfBs! \cdot nunmberOfCs!}
$$

### Counting by complement

$$
|A| = |\mathbb U|-|\bar{A}|
$$
### Product rule
$$|A \times B| = |A| \cdot |B|$$
$$\#Choices=\prod\limits^{n}_{k=1}c_k$$
### Sum rule
$$
|A \cup B| = |A| + |B|
$$
$$
(A \cap B = \varnothing)
$$
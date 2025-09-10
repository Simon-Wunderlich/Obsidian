Created: May 02 2025
Class:  [[Counting]]
- - -
Convert multi set to binary string
0 represent number of items of given type selected, 1's separate types
![[Pasted image 20250502134656.png]]
### Counting codewords
Count number of 0's and 1's
Then find permutation of multiset

$$n=\# \space of \space 0's$$
$$m=\#\space of \space 1's$$$$\frac{(n+m)!}{n! \cdot m!}$$$$\begin{pmatrix}
           n+m \\
           m
         \end{pmatrix}$$
 
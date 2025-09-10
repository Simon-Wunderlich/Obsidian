Created: May 16 2025
Class: [[Graphs]] 
- - -

For relations $R$ and $S$ of set $A$, the composition of these relations is denoted as $$R \circ S$$
where $(a,c)\in R\circ S \space$ iff there exists and element $b\in A$ such that $(a,b)\in R$ and $(b,c)\in S$
									This order matters ^^

Start with a pair of vertices such as $(a, b)$. If there exists some node that $a$ can reach in $R$ and can reach $b$ in $S$, then $(a, b)$ is in $R \circ S$. Otherwise, (a, b) is not in $R \circ S$.

![[Git/Attatchments/compOfRels.pdf|compOfRels]]
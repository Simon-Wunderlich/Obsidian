Created: Apr 04 2025
Class: [[Maths]]
- - -
#### Disjunctive normal form

$c_1$ + $c_2$ + $\cdots$ + $c_n$
where each $c_j$ is a conjunction of literals

![[Pasted image 20250404135536.png]]

Only one needs to be true for satisfaction, can be broken down into clauses

#### Conjunctive normal form

$d_1$$d_2$$\cdots$$d_n$
where each $d_j$ is a disjunction of literals

![[Pasted image 20250404135726.png]]

![[Pasted image 20250404135834.png]]
1. Write out all possibilities
		$a_1$, $a_2$, $b_1$, $b_2$
2. Factor in constraints
		![[Pasted image 20250404140015.png]]
		($a_1$+$a_2$)$\neg$($(a_1a_2)$)
		($b_1$+$b_2$)$\neg$($(b_1b_2)$)
		![[Pasted image 20250404140156.png]]
		$\neg$($a_1 \wedge b_1$)$\wedge$$\neg(a_2 \wedge b_2)$
3. Combine
	($b_1$+$b_2$)$\neg$($(b_1b_2)$) AND ($b_1$+$b_2$)$\neg$($(b_1b_2)$) AND $\neg$($a_1 \wedge b_1$) AND $\neg(a_2 \wedge b_2)$
	

Created: May 22 2025
Class: [[Modular arithmetic and factorisation]] 
- - -
Any number can be expressed as

$$
x = p_1^{a_1} \cdot p_2^{a_2} \cdots p_r^{a_r}
$$
Where $p \space is \space prime, a \in \mathbb{Z}$
### GCD and LCM from prime factorisation
Let x and y be two positive integers with prime factorisation expressed using a common set of primes as:
$$
x = p_1^{a_1} \cdot p_2^{a_2} \cdots p_r^{a_r}
$$
$$
y = p_1^{b_1} \cdot p_2^{b_2} \cdots p_r^{b_r}
$$

x divides y iff $a_i \leq b_i \forall 1 \leq i \leq r$ 
All powers of x are less than powers of y for each prime
$GCD(x,y) = p_1^{min\{a_1, b_1\}} \cdot p_2^{min\{a_2, b_2\}} \cdots p_r^{min\{a_r, b_r\}}$
$LCM(x,y) = p_1^{max\{a_1, b_1\}} \cdot p_2^{max\{a_2, b_2\}} \cdots p_r^{max\{a_r, b_r\}}$

## Primality testing
### Brute force
Check if every number from 2 to $\sqrt{x}$ divides x. If no, then x is prime

## Prime number theorum
Let $\pi (x)$ be the number of primes between 2 and x, then
$$
\lim_{x\rightarrow \infty} \frac{\pi (x)}{ \frac {x}{ln(x)}}=1
$$
Also for any integer a,
$$
Pr(a \space is \space prime) = \frac{1}{ln(x)}, a \in [2,x]
$$

Created: Oct 15 2025
Class: [[Maths]] 
- - -
# Big-O
Worst case
$$\lim_{n \rightarrow \infty} \frac{f(n)}{g(n)} < \infty$$
# Big-$\Omega$
Best case
$$\lim_{n \rightarrow \infty} \frac{f(n)}{g(n)} > 0$$
$f$ is  $\Omega(g)$ iff $g$ is $O(f)$ 
# Big-$\Theta$
Average case
f is $\theta(g)$ if constants $c_1, c_2$ exists such that
$$
c_1*g(n) \geq f(n) \geq c_2*g(n)
$$
$$
\lim_{n \rightarrow \infty} \frac{f(n)}{g(n)} = c, c \in \mathbb{R}
$$
ie f(n) and g(n) are the same complexity class of n

# Notes
$O(log_a (n) = O(log_b (n)$
as $log_a (n) = log_b (a) * log_b (n)$
and $log_b (a)$ is constant
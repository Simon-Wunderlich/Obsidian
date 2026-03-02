Created: Oct 28 2025
Class: [[Proof]] 
- - -
$$3^{n} >  2^{n}  +  n^{2}$$
$$\begin{matrix}
base case \\
3^2 > 2^2 + 2^2 = 9 > 8\\
inductive \\
3^k>2^k+k^2 \\
3^{k+1}>2^{k+1}+(k+1)^2\\
3 * (2^k+n^k) > 2 * 2^k + k^2 + 2k + 1 \\
3 * 3^k> 3^k + 2k + 3
\end{matrix}$$


$$n! \ge 2^{n}$$
$$\begin{matrix}
n! \ge 2^{n}\\
(k+1)! \ge 2^{k+1} \\
= (k+1)*k! \\
= (k+1) *2^k \\
= k*2^k + 2^k \\
= 2^{k+1} + 2^k \\
\ge 2^{k+1}
\end{matrix}$$

$$\sum_{j = 1}^n \frac{1}{j^2} \le 2 - \frac 1 n$$
$$
\begin{matrix}
\sum_{j = 1}^n \frac{1}{j^2} \le 2 - \frac 1 n \\
\frac{1}{(k+1)^2} + \sum_{j = 1}^k \frac{1}{j^2} \le 2 - \frac 1 {k+1} \\
= \frac 1 {(k+1)^2} + 2 - \frac 1 {k} \\
> \frac 1 {k(k+1)} + 2 - \frac 1 k \\
= 2 + \frac {1 - k - 1} {k(k+1)}
= 2 - \frac {1} {k+1}
\end{matrix}
$$

$$3^{n} \le (n+1)!$$
$$
\begin{matrix}
3^{k} \le (k+1)! \\
3^{k+1} \le (k+2)! \\
=3*3^k\\
= 3*(k+1)! \\
\ge (k+2)(k+1)! \\
= (k+2)!
\end{matrix}$$




$$f_n = \frac{1}{\sqrt{5}} \left[ \left( \frac{1 + \sqrt{5}}2 \right)^n - \left( \frac{1 - \sqrt{5}}2 \right)^n \right]$$

$$\begin{matrix}
\frac{1}{\sqrt{5}} \left[ \left( \frac{1 + \sqrt{5}}2 \right)^{k-2} - \left( \frac{1 - \sqrt{5}}2 \right)^{k-2} \right] + \frac{1}{\sqrt{5}} \left[ \left( \frac{1 + \sqrt{5}}2 \right)^{k-1} - \left( \frac{1 - \sqrt{5}}2 \right)^{k-1} \right]=\frac{1}{\sqrt{5}} \left[ \left( \frac{1 + \sqrt{5}}2 \right)^k - \left( \frac{1 - \sqrt{5}}2 \right)^k \right] \\
=\frac{1}{\sqrt{5}} \left[ \left( \frac{1 + \sqrt{5}}2 \right)^{k-2} - \left( \frac{1 - \sqrt{5}}2 \right)^{k-2} + \left( \frac{1 + \sqrt{5}}2 \right)^{k-1} - \left( \frac{1 - \sqrt{5}}2 \right)^{k-1} \right] \\
=\frac{1}{\sqrt{5}} \left[ \frac{(1 + \sqrt{5})^{k-2}}{2^{k-2}} - \frac{(1 - \sqrt{5})^{k-2}}{2^{k-2}}+ \frac{(1 + \sqrt{5})^{k-1}}{2^{k-1}} - \frac{(1 - \sqrt{5})^{k-1}}{2^{k-1}}  \right] \\
=\frac{1}{\sqrt{5}} \left[ \frac{(1 + \sqrt{5})^{k-2}}{2^{k-2}} - \frac{(1 - \sqrt{5})^{k-2}}{2^{k-2}}+ \frac{(1 + \sqrt{5})^{k-1}}{2^{k-1}} - \frac{(1 - \sqrt{5})^{k-1}}{2^{k-1}}  \right]
\end{matrix}$$








































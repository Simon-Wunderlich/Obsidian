Created: Mar 17 2026
Class: [[Algorithms & analysis]] 
- - -
# Backwards substitution
1. Define recurrence relation
$F(n)=F(n-1)+1$
2. Define base case
$F(1) = 0$
3.  Substitute F(n-1) until you reach base case or can identify pattern
$$\begin{matrix}
F(n) = F(n-1)+1 \\
F(n-1) = F(n-2) + 1 \\
Substitute \\
F(n) = [F(n-2) + 1] + 1 \\
=F(n-2) + 2 \\
Repeat \space for \space more \space values \space of \space n \\
F(n-2) = F(n-3) + 1  \\
F(n) = [F(n-3) + 1] + 2 \\
=F(n-3) + 3 \\
Identify \space pattern \\
F(n) =  F(n-i) + i, \space i \in [1, n]
\end{matrix}$$
4. Solve using base case
$$
\begin{matrix}
F(n) = F(n-i) + i \\
F(1) = 0 \\
Aim \space to \space eliminate \space i\\
F(n-i) = 0 \space when \space n-i = 1 \\
n-i=1 \\
i = n-1 \\
\\
Substitute \space into \space pattern\\
F(n) = F(n-i) + i \\
F(n) = F(n-[n-1])+[n-1] \\
F(n)=F(1)+[n-1]\\
Insert \space base \space case \\
F(n)=0+n-1\\
\\
F(n)=n-1\\
\end{matrix}
$$
# Empirical analysis
Just measure it lmao
When designing experiments:
1. Understand the experiment’s purpose.
2. Decide on the efficiency metric M to be measured and the
measurement unit (an operation’s count vs. a time unit).
3. Decide on characteristics of the input sample (its range, size, and
so on).
4. Prepare a program implementing the algorithm (or algorithms) for
the experimentation.
5. Generate a sample of inputs.
6. Run the algorithm (or algorithms) on the sample’s inputs and
record the data observed.
7. Analyse the data obtained.

# Rules of thumb
## O(1)
Typically algorithms or data structures whose operations does not
depend on input size.
## O(n)
Typically algorithms or data structures whose operations that
needs to evaluate most or all of the elements of an problem (input
size).
## O(n$^2$)
Typically algorithms or data structures whose operations that
needs to process/evaluate pairs of elements of an problem
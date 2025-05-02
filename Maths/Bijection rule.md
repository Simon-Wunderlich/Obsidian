Created: May 01 2025
Class: [[Counting]]
- - -
A bijection is a mapping function that maps one set to another

$x=\{a,b,c\}$
$f(x)$ is a bijection of x
$f^-1(y)$ where $y\in f(x)$ returns the corresponding element of x

if there is a bijection from set $A$ to set $B$, then the two sets have the same **cardinality**
Bijection is just the same as one to one mapping

Used to count difficult sets by mapping them to trivial sets 

### K to 1 rule
Assuming a k-1 mapping from set $A$ to $B$, then:
$$
|B|=\frac{|A|}{k}
$$
Bijection is a case of K to 1 rule 

### Converting Power set to binary 
| P(x)     | $\varnothing$ | $\{a\}$ | $\{b\}$ | $\{c\}$ | $\{a,b\}$ | $\{a,c\}$ | $\{b,c\}$ | $\{a,b,c\}$ |
| -------- | ------------- | ------- | ------- | ------- | --------- | --------- | --------- | ----------- |
| **f(x)** | 000           | 100     | 010     | 001     | 110       | 101       | 011       | 111         |

| x                | a   | b   | c   |
| ---------------- | --- | --- | --- |
| f($\varnothing$) | 0   | 0   | 0   |
| f(a)             | 1   | 0   | 0   |
| f(b)             | 0   | 1   | 0   |
| f(c)             | 0   | 0   | 1   |
| f(a,b)           | 1   | 1   | 0   |
| f(a,c)           | 1   | 0   | 1   |
| f(b,c)           | 0   | 1   | 1   |
| f(a,b,c)         | 1   | 1   | 1   |
If element is present as parameter, the bit in its index in the string is 1, else 0
Created: May 01 2025
Class: [[Maths]] 
- - -
$x=\{a,b,c\}$
f(x) is a bijection of x

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
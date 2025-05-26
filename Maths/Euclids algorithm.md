Created: May 22 2025
Class: [[Modular arithmetic and factorisation]] 
- - -
Finds GCD for integers x and y
```python
#x > y
def euclid(x, y):
	r = x mod y
	if r == 0:
		return y
	else
		return euclid(y,r)
```
Uses the fact that
$$
GCD(x,y)=GCD(y \space mod \space x, x)
$$


### Extended euclids algorithm
#unsure
Let x and y be integers, there are always integers s and t such that
$$
GCD(x,y) = sx + ty
$$
Using euclid's algo, compute GCD, noting down each value of y
Take last two values and rearrange their mod equation from $x \space mod \space y$ to $x - (x \space div \space y) \cdot y$ 
Use simultaneous equation to solve for s, t

![[Git/Attatchments/extendedEuclidsAlgorithm.pdf|extendedEuclidsAlgorithm]]


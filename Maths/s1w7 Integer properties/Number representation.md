Created: May 23 2025
Class: [[Modular arithmetic and factorisation]] 
- - -
### Representation
Every int n can be represented as 
$$
n=a_k\cdot b^k + a_{k-1}\cdot b^{k-1} + \cdots + a_0\cdot b^0
$$
Where $a^i$ represents a digit in int n and b represents the base of int n
Such that $n=(a_k\cdot a_{k-1} \cdots a_0)_b$ 

### Convert decimal to different base
``` python
base = #user input
async binary(dec)
	print(dec mod base)
	d = dec div base
	
	if(d == 0)
		return
```

![[Git/Xournal/decToBin.pdf|decToBin]]

### Number of digits required to represent number
Given integer n and base b, number of digits $k = \lceil log_b (n+1) \rceil$  
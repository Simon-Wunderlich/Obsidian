Created: May 23 2025
Class: [[Modular arithmetic and factorisation]] 
- - -
``` python
async binary(dec, mods : stack)
	m = dec mod 2
	d = dec div 2

	if(d == 0)
		return mods.join("")
	else
		mods.push(m)
		return binary(d, mods)
```
![[Git/Xournal/decToBin.pdf|decToBin]]
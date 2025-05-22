Created: May 22 2025
Class: [[Integer properties]] 
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


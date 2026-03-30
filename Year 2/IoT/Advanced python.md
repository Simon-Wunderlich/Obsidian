Created: Mar 30 2026
Class: [[IoT]] 
- - -
# Static
```python
class test():
	@staticmethod
	def AH():
		print("oooooh")
		
test.AH()
```

# Duck typing
Lax typing
Kinda in-built polymorphism
```python
class A():
	def AG():
		print("svrvs")
class B():
	def AG():
		print("bdzdvbareb")
		
for x in [A(), B()]:
	x.AG()
```

# Iterators
Contains value and next method. When nothing to return, throws StopIteration exception
```python
class A():
	# Define start values
	__iter__():
		self.value = 10
	
	# Define next item
	__next__():
		if (self.value < 0):
			raise StopIteration
			
		self.value -= 1
		return self.value
		
for x in A():
	print(x)
```

# Yield
Function containing yield
```python
def test():
	for x in range(10):
		yield x
		
for x in test():
	print(x)
```

# Closures(?)
Combo of function and set of references to variables in the functions scope
```python
def etbn():
	g= 0
	
AH = etbn()

print(AH.__closure__[0].g)
```


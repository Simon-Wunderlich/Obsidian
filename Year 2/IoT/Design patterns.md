Created: Mar 30 2026
Class: [[IoT]] 
- - -
# Pattern programming
## Cohesion
Keep the tasks and responsibilities for a class closely related. Don't cram everything into one big task
## Coupling
Dependency between each class. How much they rely on each other
## Encapsulation
[[Inheritance]]

# Decorators
Wrap target function, doesn't modify function itself
```python
def dec(func):
	def wrapper():
		print("before")
		func()
		print("after")
		
	return wrapper
	
@dec
def run():
	print("run")
	
```

# Factory
Creates objects without exposing logic to client and referring to the newly created object using a common interface.
```python
class A():
	def run():
		print("A")
class B(A):
	def run():
		print("B")
		
class C(A):
	def run():
		print("B")
		
class factory():
	@staticmethod
	def createObj(self, type):
		# Obj assignment is hidden from main
		match (type):
			case "old one":
				return B()
			case "new one":
				return C()
			default
				return globals()[type]
	
def main():
	clases = ["old one", "new one"]
	for x in clases:
		# Simple interface for each class, regardless of complexity when actually creating the objects
		factory.createObj(x).run()
```
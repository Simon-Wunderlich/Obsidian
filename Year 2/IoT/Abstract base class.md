Created: Mar 16 2026
Class: [[IoT]] 
- - -
```python
from abc import ABC, abstractmethod
class parent():
	@abstractmethod
	def hello():
		print("hi")
	
class child(parent):
	def hello():
		super().hello()
		print("hello")
```



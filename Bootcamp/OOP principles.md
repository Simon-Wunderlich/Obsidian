Created: Apr 09 2025
Class: [[Bootcamp]]
- - -
### Inheritance
``` java
abstract class parent {
	String property;
	//Must be implemented by child classes
	abstract void print();
}

class child extends parent {
	//Override used to modify parent methods
	@Override
	void print() {
		//Access parent variables with super.{var name}
		System.out.println(super.property);
	}
}
```
### Interface
```java
interface IclassA {
	void print(); //imlpicitly public and abstract
}

public classA implements IclassA {
	...
} 
```

![[Pasted image 20250409154203.png]]

![[Pasted image 20250409154221.png]]

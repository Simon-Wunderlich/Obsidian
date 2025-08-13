Created: Aug 07 2025
Class: [[Bootcamp]] 
- - -
# Types of constructors
```cpp
//Standard constructor
MyClass(int _a)
{
	a = _a;
}

//Move constructor
MyClass(int _a) a(_a) {}

//Copy constructor
MyClass(MyClass& _myClass){
	dataObject = new int;
	dataObject = *_myClass;
}

//Deconstructor
~MyClass()
{
	delete dataObject;
}
```


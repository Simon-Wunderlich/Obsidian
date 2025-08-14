Created: Aug 07 2025
Class: [[Bootcamp]] 
- - -
# Standard constructor
```cpp
MyClass(int _a)
{
	a = _a;
}
```

# Move constructor
```cpp
MyClass(int _a) a(_a) {}

```

# Copy constructor
```cpp
//Copy constructor
MyClass(MyClass& _myClass){
	dataObject = new int;
	dataObject = *_myClass;
}
```

# Deco
```cpp

//Deconstructor
~MyClass()
{
	delete dataObject;
}
```


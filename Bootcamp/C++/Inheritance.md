Created: Aug 24 2025
Class: [[Bootcamp]] 
- - -
## Static binding
#### Compile-time polymorphism
```cpp
class Base
{
	public:
		Base(int _x) : x(_x) {}
		void print() {
			std::cout << "BASE";
		}
	private:
		int x;
}

class Child : public Base
{
	public:
		
		Child(int _x, int _y) : Base(_x), y(_y) {}
		
		void printAll()
		{
			Base::print();
			print();
		}
		void print()
		{
			std::cout << "CHILD";
		}
	private:
		int y;
}

Child c = Child();
c.printAll();
//Output: BASECHILD
```

## Virtual functions
#### Runtime polymorphism
Used for when the compiler cannot determine class. eg 
```cpp
class Base
{
	public:
		virtual void print() {}
}

class ChildA : public Base
{
	public:
		void print()
		{
			std::cout << "A";
		}
}

class ChildB : public Base
{
	public:
		void print()
		{
			std::cout << "B";
		}
}

std::vector<Base*> vec;
vec.push_back(new ChildA());
vec.push_back(new ChildB());
for(Base* b : vec)
{
	b->print();
}
//Output: CHILD
```

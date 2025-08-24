Created: Aug 24 2025
Class: [[Bootcamp]] 
- - -
```cpp
class Base
{
	public:
		void print() {
			std::cout << "BASE";
		}
}

class Child : public Base
{
	public:
		void printAll()
		{
			Base::print();
			print();
		}
		void print()
		{
			std::cout << "CHILD";
		}
}

Child c = Child();
c.printAll();
//Output: BASECHILD
```
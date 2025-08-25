Created: Aug 24 2025
Class: [[Bootcamp]] 
- - -
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
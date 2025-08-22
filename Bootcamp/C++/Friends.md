Created: Aug 22 2025
Class: [[Bootcamp]] 
- - -

Friend function of class is a non member function of a class that can:
- Access both private and public class members
- Be applied to functions, classes, or member functions of other classes

```cpp
class A
{
	private:
		int num = 5;
}

class B
{
	private:
		int _num = 5;
		
	public:
		//Non-Member function
		int _num = 5;
		friend void func(A _a, B _b)
		
		//Whole class as friends
		friend class A;
}

void func(A _a, B _b)
{
	std::cout << _a.num == _b.num;
}

A a;
B b;

func(a,b); //Output: 5

b.A = a;
std::cout << b.A.num; //Output: 5

```

## Controlled usage
### Whole class friend
Used for when two classes need comprehensive access

### Non-member function friends
Used for more specific operations such as comparisons or manipulations
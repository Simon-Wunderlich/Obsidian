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
	public:
		friend void func(A _a)
		{
			std::cout << a;
		}
}

A a;
B b;

b.func(a); //Output: a
```

## Controlled usage
### Whole class friend
Used for when two classes need comprehensive access

### Non-member function friends
Used for more spceific operations such as comparisons or manipulations
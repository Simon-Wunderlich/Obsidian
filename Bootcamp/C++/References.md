Created: Aug 22 2025
Class:  [[Bootcamp]]
- - -
```cpp
void test(int& num)
{
	num++;
}

int main()
{
	int number = 5;
	test(number);
	std::cout << number; // 6
}
```
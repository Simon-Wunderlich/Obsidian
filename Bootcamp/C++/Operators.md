Created: Aug 22 2025
Class: [[Bootcamp]] 
- - -
# Comparison

```cpp
bool Object::operator==(const Object& other)
{
	return this->prop == other.prop;
}

bool Object::operator<(const Object& other)
{
	return this->prop < other.prop;
}

//etc
```

# +
```cpp
Object& Object::operator+(std::string s)
{
	this -> prop.push_back(s);
	return *this;
}
```

# Streams
## <<
```cpp
Object& operator<<(std::string& s)
{
	this -> prop.push(s);
	return *this;
}

//or

std::ostream& operator<<(std::ostream& os, const Object obj)
{
	os << obj.prop;
	return os;
}
```
## >>
```cpp
Object& operator>>(std::string s)
{
	s = this-> prop.front();
	this->prop.pop();
	return *this;
}

//

std::istream& operator>>(std::istream& is, const Object obj)
{
	is >> obj.prop;
	return is;
}
```

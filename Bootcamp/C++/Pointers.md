Created: Sep 13 2025
Class: [[]] 
- - -
# Initialisation
```cpp
//ref_x is a reference to x
//ref_x mem addr is same as x
int* ref_x = &x;
```

# Accessing data
```cpp
std::cout << ref_x; //Outputs x memory address
std::cout << *ref_x; //Outputs x value
```

# Dereferencing
```cpp
Object* ptr = &example;
ptr -> exampleMethod(); //Calls method of Object
(*ptr).exampleMethod(); //Calls method of Object
```


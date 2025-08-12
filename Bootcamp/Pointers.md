```cpp
//ref_x is a reference to x
//ref_x mem addr is same as x
int* ref_x = &x;
std::cout << ref_x; //Outputs x memory address
std::cout << *ref_x; //Outputs x value

Object* ptr = &example;
ptr -> exampleMethod(); //Calls method of Object
```


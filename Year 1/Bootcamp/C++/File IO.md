Created: Aug 13 2025
Class: [[Bootcamp]] 
- - -
# Read
```cpp
// Create a text string, which is used to output the text file  
std::string myText;  
  
// Read from the text file  
std::ifstream MyReadFile("filename.txt");  

// Use a while loop together with the getline() function to read the file line by line  
while (std::getline (MyReadFile, myText)) {  
  // Output the text from the file  
  std::cout << myText;  
}  
  
// Close the file  
MyReadFile.close();
```

# Write
```cpp
std::ofstream MyReadFile("filename.txt");  
MyReadFile << "HeeHee";
MyReadFile.close();
```
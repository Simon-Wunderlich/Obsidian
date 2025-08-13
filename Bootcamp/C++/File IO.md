Created: Aug 13 2025
Class: [[Bootcamp]] 
- - -
```cpp
// Create a text string, which is used to output the text file  
string myText;  
  
// Read from the text file  
ifstream MyReadFile("filename.txt");  
  
// Use a while loop together with the getline() function to read the file line by line  
while (getline (MyReadFile, myText)) {  
  // Output the text from the file  
  cout << myText;  
}  
  
// Close the file  
MyReadFile.close();
```

Created: Apr 09 2025
Class: [[Bootcamp]]
- - -

### Write
``` java
import java.io.PrintWriter;

public class Main {  
    public static void main(String[] args) throws IOException {  
        //Will create file if not found  
        PrintWriter pw = new PrintWriter("output.txt");  
        pw.print("Helo, World!");  
        pw.close();  
    }  
  
}
```

### Read
``` java 
import java.io.FileStream;
import java.util.Scanner;

public class Main {
	public static void main(String[] args) throws IOException {
		FileStream fs = new FileStream("input.txt");
		Scanner scnr = new Scanner(fs);
		
		scnr.nextLine();
		...
		fs.close(); 
	}

}
```

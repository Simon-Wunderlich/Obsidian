Created: Apr 09 2025
Class: [[Bootcamp]]
- - -

### Write
``` java
import java.io.PrintWriter;
import jaba.io.BufferedWriter;

public class Main {  
    public static void main(String[] args) throws IOException {  
        //Will create file if not found  
        boolean append = ___
        BufferedWriter pw = new BufferedWriter(new PrintWriter("output.txt"), append);  
        pw.write("Helo, World!");  
        pw.close();  
    }  
  
}
```

### Read
``` java 
import java.io.FileReader;
import java.util.Scanner;
import java.io.BufferedReader;

public class Main {
	public static void main(String[] args) throws IOException {
		
		BufferedReader reader = new BufferedReader(new FileReader("input.txt"));
		
		reader.readLine();
		...
		reader.close(); 
	}

}
```


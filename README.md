# Java_CheatSheet

#### Reading a Text File


```java
import java.util.Scanner;
import jhava.nio.file.Paths;

try(Scanner scanner = new Scanner(Paths.get("file.txt"))) {
  while (scanner.hasNextLine()) {
    String row = scanner.nextLine();
    System.out.println(row);
  }
} catch (Exception e) {
  System.out.println("Error: " + e.getMessage());
}
```
#### Skipping empty line

```java
// if the line is blank we do nothing
if (line.isEmpty()) {
    continue;
}
```

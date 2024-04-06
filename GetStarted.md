### Step1: Import the utilities
```java
  import java.util.*;
```

### Step2: Defining a class
```java
public class GetStarted{.....}
```
- Class Name: It should start with a capital letter and use camel case if the name consists of multiple words.
- iIt can be public, private, protected, or default (no modifier). Choose an appropriate access modifier 

### Step3: Main method, where the program starts executing
```java
public static void main(String[] args) {
    // Main method contents go here
}

```
- Accessibility: The main method must be declared as public so that it can be accessed by the Java runtime system.
- Static Modifier: The main method must be declared as static because it belongs to the class rather than to any specific instance of the class.
- Return Type: The main method has a return type of void, which means it does not return any value
- Method Name: The method name is main, which is a special name recognized by the Java runtime system to identify the entry point of the program.
- String[] args: The args parameter is an array of strings containing the command-line arguments provided when running the program.

### Step4: Take input from the user - Number, Strings and storing it in arrays
  - Creating a Scanner object named "scanner" to read input from the console
    ```java
     Scanner scanner = new Scanner(System.in);
    ```
  - Prompting the user to print
    ```java
    System.out.println("Enter values");
    ```
 - Reading the number entered by the user and storing it in the variable "n"
    ```java
    int n = scanner.nextInt();
    ```
- Creating an array to store
  ```java
  int[] array_num = new int[n];
  ```

- Example1: Asking the user to enter the length of the array followed by numbers to be stored in an array.
  Input Format
  5 /n
  1 10 42 13 5
  
  ```java
  Scanner scanner = new Scanner(System.in);
  int n = scanner.nextInt();
  int[] arr1 = new int[n];
  for (int i = 0; i < n; i++) {
            arr1[i] = scanner.nextInt();
        }
  ```
- Example2: If you want to read a string entered by the user and store it in the variable "name" along with creating an array:
  Input Format
  Alice Bob Kelly John

   ```java
    System.out.println("Enter names:");
    String name = scanner.nextLine();
    String[] namesArray = name.split(" "); // assuming names are space-separated
  ```



### Step5: Iterating over Numbers, Strings, Arrays
#### Iterating over number
```java
  for (int i = 1; i <= 10; i++) {
    System.out.println(i);
    }
```
#### Iterating over String
- Example1:
```java
  String message = "Hello";
  
  // Using a traditional for loop
  for (int i = 0; i < message.length(); i++) {
      System.out.println(message.charAt(i));
  }
  
  // Using an enhanced for loop
  for (char ch : message.toCharArray()) {
      System.out.println(ch);
  }

```
  - Example2: comparing each character of a string
  ```java
    for (int i = 0; i< name.length(); i++){
                char ch = name.charAt(i);
                if (ch == 'z') {
                    countz++;
                    
                }
    }
  ```

- Example3: Taking input in a single line as a string, converting into integer.
  ```java
        Scanner scanner = new Scanner(System.in);
        String[] cost = scanner.nextLine().split(" ");
        int cost_green = Integer.parseInt(cost[0]);
        int cost_purple = Integer.parseInt(cost[1]);
  ```
- Example4: Taking numbers as input and looping the digits, by storing it in string , converting to char array
```java

        Scanner scanner = new Scanner(System.in);
        String Input = scanner.nextLine();
        char[] Characters = Input.toCharArray();
        for (int i = 0; i < Characters.length; i++){
            char c = Charachers[i];
            System.out.println(c);
        }
```

#### Iterating over Arrays
```java
for (int i = 1; i <= 10; i++) {
    System.out.println(i);
    }
```

- Example1: Taking input in single line as a string, converting it to integer and storing it in a 2D array, num is length of array.
```java
        int num = Integer.parseInt(scanner.nextLine());
        int [][] arr2 = new int[num][2];
        for (int i =0; i<num; i++ ) {
            String[] scoreStr = scanner.nextLine().split(" ");
            arr2[i][0] = Integer.parseInt(scoreStr[0]);
            arr2[i][1] = Integer.parseInt(scoreStr[1]);
        }
            for (int i = 0; i < num; i++) {
                System.out.println("Output: " + arr2[i][0] + " " + arr2[i][1]);
            }
```


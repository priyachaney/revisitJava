### Step1: Import the utilities
```java
  import Java.utils.*;
```

### Step2: Defining a class
```java
public class GetStarted{.....}
```
- Class Name should start with camel case
- identifer of the class should be defined accordingly - public , private

### Step3: Main method, where the program starts executing
```java
-  public static void main(String[] args) {....}
```

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
- For example1, if you want to read a string entered by the user and store it in the variable "name" along with creating an array:

 ```java
  System.out.println("Enter names:");
  String name = scanner.nextLine();
  String[] namesArray = name.split(" "); // assuming names are space-separated
```

### Step5: Iterating over Numbers, Strings, Arrays

- Iterating over number
```java
  for (int i = 1; i <= 10; i++) {
    System.out.println(i);
    }
```
- Iterating over String
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
- Iterating over Arrays
```java
for (int i = 1; i <= 10; i++) {
    System.out.println(i);
    }
```




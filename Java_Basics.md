### Variables and Data Types:

- Declare and initialize variables: `int x = 5;`
- Primitive data types: `int`, `double`, `boolean`, `char`, etc.
- Reference data types: `String`, `Object`, `Array`, etc.

### Input and Output:

- Reading input from the console
  ```java
  Scanner scanner = new Scanner(System.in);
  int number = scanner.nextInt();
  String text = scanner.nextLine();

### String 
- Creation and initialization: String str = "Hello";
- String methods: length(), charAt(), substring(), indexOf(), equals(), etc.
- StringBuilder for mutable strings:

 ```java
StringBuilder sb = new StringBuilder("Hello");
sb.append(" World");
 ```

### String Manipulation:

1. **String Comparison:**
   - Ignore case: 
     ```java
     boolean isEqualIgnoreCase = str1.equalsIgnoreCase(str2);
     ```
   - Compare to another string: 
     ```java
     int comparison = str1.compareTo(str2);
     ```

2. **String Searching:**
   - Index of substring: 
     ```java
     int index = str.indexOf(subStr);
     ```
   - Last index of substring: 
     ```java
     int lastIndex = str.lastIndexOf(subStr);
     ```
   - Check if string contains a substring: 
     ```java
     boolean containsSubStr = str.contains(subStr);
     ```
   - Check if string starts/ends with a substring: 
     ```java
     boolean startsWith = str.startsWith(subStr);
     boolean endsWith = str.endsWith(subStr);
     ```

3. **String Modification:**
   - Convert to upper/lower case: 
     ```java
     String upperCase = str.toUpperCase();
     String lowerCase = str.toLowerCase();
     ```
   - Replace characters/substrings: 
     ```java
     String replaced = str.replace(oldChar, newChar);
     ```

4. **String Splitting and Joining:**
   - Split string into array: 
     ```java
     String[] parts = str.split(delimiter);
     ```
   - Join array elements into a string: 
     ```java
     String joined = String.join(delimiter, parts);
     ```
   - Tokenizing string: 
     ```java
     StringTokenizer tokenizer = new StringTokenizer(str, delimiter);
     while (tokenizer.hasMoreTokens()) {
         String token = tokenizer.nextToken();
         // Process token
     }
     ```

5. **String Trimming:**
   - Trim leading and trailing whitespace: 
     ```java
     String trimmed = str.trim();
     ```

6. **String Formatting:**
   - Format string with placeholders: 
     ```java
     String formatted = String.format("Name: %s, Age: %d", name, age);
     ```
   - Padding string with spaces: 
     ```java
     String padded = String.format("%-10s", str);
     ```

7. **String Building:**
   - Building string dynamically: 
     ```java
     StringBuilder builder = new StringBuilder();
     builder.append("Hello");
     builder.append("World");
     String result = builder.toString();
     ```

8. **Regular Expressions:**
   - Pattern matching and manipulation using regex:
     ```java
     Pattern pattern = Pattern.compile(regex);
     Matcher matcher = pattern.matcher(str);
     boolean matches = matcher.matches();
     ```

### Array 
- Declaration and initialization: int[] numbers = {1, 2, 3};
- Accessing elements: int x = numbers[0];
- Iterating through arrays:
 ```java
for (int i = 0; i < numbers.length; i++) {
    System.out.println(numbers[i]);
}
```
### Array Manipulation:

1. **Creating Arrays:**
   - Declare and initialize: 
     ```java
     int[] arr = {1, 2, 3};
     ```
   - Specify size and initialize: 
     ```java
     int[] arr = new int[5];
     ```

2. **Accessing Elements:**
   - Access by index: 
     ```java
     int element = arr[index];
     ```
   - Modify elements: 
     ```java
     arr[index] = newValue;
     ```

3. **Array Length:**
   - Get length: 
     ```java
     int length = arr.length;
     ```

4. **Iterating Arrays:**
   - Using for loop: 
     ```java
     for (int i = 0; i < arr.length; i++) {
         // Access and process arr[i]
     }
     ```

5. **Array Copying:**
   - Copy array elements: 
     ```java
     int[] newArr = Arrays.copyOf(arr, arr.length);
     ```

6. **Searching and Sorting:**
   - Binary search: 
     ```java
     int index = Arrays.binarySearch(arr, key);
     ```
   - Sorting: 
     ```java
     Arrays.sort(arr);
     ```

### Core Java Concepts:

1. **Object-Oriented Programming:**
   - Classes and objects
   - Inheritance
   - Polymorphism

2. **Exception Handling:**
   - try-catch-finally blocks
   - Checked vs. unchecked exceptions

3. **Collections Framework:**
   - Lists, sets, maps
   - Iterators
   - Comparable and Comparator interfaces

4. **Multithreading:**
   - Thread creation and management
   - Synchronization
   - Thread safety

5. **Input-Output (I/O):**
   - Streams (FileInputStream, FileOutputStream)
   - Readers and Writers

6. **Generics:**
   - Type safety
   - Generic classes and methods

7. **Annotations:**
   - Built-in annotations (@Override, @Deprecated)
   - Custom annotations

8. **String Handling:**
   - String comparison and manipulation
   - Regular expressions

9. **Date and Time API:**
   - LocalDate, LocalTime, LocalDateTime
   - Formatting and parsing

10. **Lambda Expressions:**
    - Functional interfaces
    - Syntax and usage
